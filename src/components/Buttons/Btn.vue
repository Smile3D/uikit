<template>

    <button
      :class="`btn ${additionalClass} ${textColor}`"
    >{{ textBtn }}</button>

</template>

<script>
export default {
  name: 'Btn',
  props: {
    additionalClass: String,
    textBtn: String,
    textColor: String
  }
}
</script>

<style scoped lang="scss">
.btn {
  transition: background-color 0.3s;
  box-sizing: border-box;
  display: flex;
  align-items: center;
  justify-content: center;
  border: none;
  min-width: 200px;
  min-height: 40px;
  border-radius: 40px;
  padding: 10px 20px;
  font-size: 14px;
  letter-spacing: 1px;
  text-transform: uppercase;
  font-weight: 600;
  background-color: transparent;
  cursor: pointer;

  &--bg-primary {
    background-color: blue;

    &:hover {
      background-color: orange;
    }
  }

  &--bg-secondary {
    background-color: orange;

    &:hover {
      background-color: blue;
    }
  }

  &--color-text-primary {
    color: #fff;
  }

  &--color-text-secondary {
    color: blue;
  }

  &--outline {
    border: 1px solid blue;

    &:hover {
      background-color: blue;
      color: #fff;
    }
  }
}
</style>
