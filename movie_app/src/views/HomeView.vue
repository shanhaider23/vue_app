<template>
  <div class="home">
   <div class="feature-card">
    <router-link to="/movies/tt3896198">
      <img  src="https://images.unsplash.com/photo-1616530940355-351fabd9524b?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=735&q=80" class="feature-img" alt="n" />
      <div class="detail">
        <h3>Hello</h3>
        <p>yes</p>
      </div>

    </router-link>

   </div>
   <form @submit.prevent="" class="search-box"> 
    <input type="text" placeholder="Search" />
    <input type="submit" value="Search" />
   </form>
    <div class="movies-list"></div>
  </div>
</template>

<script>


export default {
  
}
</script>
<style lang="scss">
  .home{
    .feature-card {
      position: relative;
      .feature-img {
        display: block;
        width: 100%;
        height: 300px;
        object-fit: cover;
        position: relative;
        z-index: 0;
      }
      .detail{
        position: absolute;
        left: 0;
        right: 0;
        bottom: 0;
        background-color: rgba(0 , 0, 0, 0.6);
        padding: 16px;
        z-index: 1;

        h3{
          color: #fff;
          margin-bottom: 16px;
        }
        p{
          color: #fff;
        }
      }
    }
    .search-box {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 16px;

       input{
        display: block;
        appearance: none;
        border: none;
        outline: none;
        background: none;
        &[type="text"] {
          width: 100%;
          color: #fff;
          background: #496583;
          font-size: 20px ;
          padding: 10px 16px;
          border-radius:8px ;
          margin-bottom: 15px;
          transition: 0.4s;
          &::placeholder {
            color: #f3f3f3;

          }
          &:focus{
            box-shadow: 0px 3px 6px rgda (0, 0, 0, 0.2);
          }

        }

       }

    }
  }
</style>