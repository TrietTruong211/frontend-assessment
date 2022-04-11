<template>
  <div class="item__container">
    <div class="item__container-inner">
      <h1>Bonus Questions</h1>
      <p>
        Explain why the result of ('b' + 'a' + + 'a' + 'a').toLowerCase() is
        banana
      </p>
      <p>('b' + 'a' + + 'a' + 'a') is compiled from left to right</p>
      <p>('b' + 'a' + + 'a' + 'a') the first operation is 'b' + 'a' = 'ba'</p>
      <p>
        ('ba' + + 'a' + 'a') the second operation is 'ba' + (+ 'a'), where (+
        'a') results in "Not a number" ie "NaN" since 'a' is a string
      </p>
      <p>
        ('ba' + 'NaN' + 'a') NaN is treated as string, and 'ba' + 'NaN' =
        'baNaN'
      </p>
      <p>
        ('baNaN' + 'a') this is a normal string concatenation operation, results
        in 'baNaNa'
      </p>
      <p>And the whole string is transformed to lower case, hence 'banana'</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "BonusQuestions",
  components: {},
};
</script>
