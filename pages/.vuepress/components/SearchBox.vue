<template>
    <section class="input-control">
        <input type="search" id="search" placeholder="enter keywords of project name"/>
        <button>Find</button>
    </section>
</template>

<script>
export default{
    
}
</script>

<style>
    *{
        font-family: Nunito, sans-serif;
    }

    .input-control{
        width: 100%;
        display: flex;
        flex-direction: row;
        justify-content: flex-start;
    }

    .input-control *{
        padding: 10px 20px;
    }

    input{
        flex-grow: 1;
        border:1px solid #777;
        outline:none;
        border-right: none;
    }

    input:focus{
        outline: none;
    }

    button{
        border:1px solid #777;
        border-left: none;
        outline: none;
        background-color: #00CEFF;
    }

    button:hover{
        background-color: #2E5A97;
        color:white;
    }
</style>