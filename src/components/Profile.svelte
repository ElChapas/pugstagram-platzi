<script>
    export let nickname;
    export let name;

</script>

<style>
  .Profile-content {
    display: flex;
    align-items: center;
  }
  .Profile-avatar img {
    width: 42px;
    height: 42px;
    border-radius: 50%;
  }
  .Profile-info {
    margin: 0 0 0 0.5em;
  }
  .Profile-info h2 {
    font-size: 14px;
    color: black;
    margin: 0;
    padding: 0;
  }
  .Profile-info span {
    font-size: 12px;
    font-weight: normal;
  }
</style>

<div class="Profile">
    <div class="Profile-content">
        <div class="Profile-avatar">
            <img src="https://scontent.felp1-1.fna.fbcdn.net/v/t1.0-9/p960x960/72267831_1678206565647907_8930515139111682048_o.jpg?_nc_cat=109&_nc_sid=85a577&_nc_oc=AQkMwbImfX1aAxiUbXdey4xDlS_ebx4wkgL52zcx2VOGmiQ_aPxfjkzZs39AcZT6qyo&_nc_ht=scontent.felp1-1.fna&_nc_tp=6&oh=4b081dc5172b3c14847020ef16ca551e&oe=5EBE00FB" alt="">
        </div>
        <div class="Profile-info">
            <h2>{nickname}</h2>
            <span>{name}</span>
        </div>
    </div>
</div>