<script>
    import "@picocss/pico";
    import CardButton from "../lib/CardButton.svelte";
    import Question from "../lib/Question.svelte";
    import Stopwatch from "../lib/Stopwatch.svelte";
    import StartModal from "../lib/StartModal.svelte";
    import { answer } from "../answerStore"

    let array = [1, 63, 81, 19];
    let num1 = 1;
    let num2 = 1;
    let ans = 0;
    let score = 0;

    const checkAns = (n) => {
      if((n == ans)&&(n != -3)){
        score += 10
      }else if ((n != ans)&&(n != -3)){
        score -= 5
      }
    }

    const genQ = (n) => {
      checkAns(n)
      num2 = Math.floor(Math.random()*12)
      num1 = Math.floor(Math.random()*12)
      array[Math.floor(Math.random()*3)] = num1*num2
      ans = num1*num2
      answer.set(-3)
    }


    answer.subscribe(val=>{
        genQ(val)
    })
</script>

<div style="height:100%;">
  <div style="display: flex; justify-content:space-between; padding: 15px;">
    <h3>Score: {score}</h3>
    <Stopwatch score={score} />
  </div>
  <main>
    <StartModal />
    <Question question={`${num1} x ${num2}`} />
    <CardButton answers={array}/>
  </main>
</div>

<style>
  main {
    display: flex;
    height: 50%;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
</style>