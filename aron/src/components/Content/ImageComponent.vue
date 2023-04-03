  <template>
    <h3 class="ClientText">{{text}}</h3>
    <div class="ComboTextPhoto">
      <img :src=imageSrc class="ClientImage"/>
      <h3 class="ClientText2">{{text}}</h3>
    </div>
</template>
  <script lang="ts">
export default {
    props: {
      imageSrc: String,
      text: String
    }
  }
</script>

<style>
.ClientImage{
    width: 100%;
    height: 100%;
    object-position: 50% 0%;
}

.ClientText{
        z-index: 0;
    opacity: 1;
    position: absolute;
    text-align: center;
    vertical-align: middle;
    color:#d6d1ca;
    font-family: 'Source Sans 3', sans-serif;
    text-transform: uppercase;
    font-size: 94px;
    margin-left: -36px;
    margin-top: 233px;
    background: none;


}
.ComboTextPhoto{
    position: relative;
    display: flex;
    overflow: hidden;
    max-width: 100%;
    margin-right: auto;
    margin-left: auto;

    align-items: center
}
.ClientText2{
    z-index: 2;
    color: #ffea00;
    font-family: 'Source Sans 3', sans-serif;
    text-transform: uppercase;
    font-size: 94px;
    opacity: 1;
    position: absolute;
    text-align: center;
    vertical-align: middle;
    background: none;
    width: 600px;
    margin-left: -74px;
    margin-top: 96px;
}
</style>
