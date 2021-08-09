<template>
    <div id="Profil" class="profil_container">
        <div class="pdp">
            <img :src="$parent.ourData['img_profil']" alt="">
            <img src="@/assets/filtre_pdp.svg" alt="">
            <p>Current Student</p>
        </div>
        <div class="description">
            <div class="name_container">
                <h1>{{$parent.ourData['firstname']}} {{$parent.ourData['lastname']}}</h1>
                <div>
                    <p>{{$parent.ourData['age']}}</p>
                    <p class="gender">{{$parent.ourData['gender']}}</p>
                    <p class="city">{{$parent.ourData['city']}}</p>
                </div>
            </div>
            <p>
                {{$parent.ourData['description']}}
            </p>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Profil',
}
</script>
<style scoped>

.profil_container {
    width: 100%;
    height: 100%;
    background-color: white;

}

/* géstion de la photo de profil */
.pdp {
    position: relative;
    width: 100%;
    height: 60%;
}
.pdp img {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    object-fit: cover;
}
.pdp img:first-child {
    height: 100%;
}
.pdp p {
    position: absolute;
    background-color: rgba(0, 0, 0, .25);
    top : 33px;
    left: 42px;
    border-radius: 3px;
    padding: 2px 9px 2px 9px;
    color: white;
    font-size: 14px;
}

/* géstion de la déscription */

.description {
    width: 100%;
    height: 30%;
    padding: 10% 10% 0% 10%;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}


.name_container {
    width: max-content;
    height: 40%;
    display: flex;
    flex-direction: column;
    justify-content: space-around;

}
.name_container h1 {
    font-size: 32px;
}
.name_container div {
    display: flex;
    justify-content: space-between;
}
.gender {
    background-color: #FFEAEB;
    border-radius: 3px;
    padding: 2px 9px 2px 9px;
    color: #D0004B;
    font-size: 14px;
}
.city {
    background-color: #E8FBED;
    border-radius: 3px;
    padding: 2px 9px 2px 9px;
    color: #089C67;
    font-size: 14px;
}

</style>
