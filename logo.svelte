<script lang="ts">
   import logo from './logo.png';

   function openMyGitHubAndLinkedin() {
      window.open("https://www.linkedin.com/in/dev-icaroglauco/", '_blank');
      window.open("https://github.com/icaroglauco-lab", '_blank').focus();
   }

</script>

<img src="{logo}" class={$$props.class} on:click={openMyGitHubAndLinkedin} title="Open my linkedin and my github" alt="Open my linkedin and my github">

<style lang="sass">
   img
      width: 100px
      height: 100px
      padding: 3px
      border-radius: 50%
      animation: 2s
      cursor: pointer
      animation-name: none 0

      &:hover
         animation-name: spin
         animation-iteration-count: 1

   @keyframes spin
      0%
         transform: rotate(0deg)
      100% 
         transform: rotate(360deg)
         animation-play-state: pause
         
</style>