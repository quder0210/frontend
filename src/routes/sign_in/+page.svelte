<script lang="ts">
  const login = () => {
    alert("로그인 성공!");
  };
</script>

<main>
  <div>
    <div id="loginContainer">
      <div id="idInputContainer">
        <input type="text" id="idInput" placeholder="아이디를 입력해주세요." />
      </div>
      <div id="passwordContainer">
        <input
          type="password"
          id="password"
          placeholder="비밀번호를 입력해주세요."
        />
      </div>
      <a href="main" on:click={login}>
        <div id="loginButton">로그인</div>
      </a>
    </div>
  </div>
</main>

<style>
  a {
    text-decoration: none;
    color: white;
  }
  #loginContainer {
    margin: auto;
    width: 600px;
    background-color: rgb(59, 56, 56);
    text-align: center;
    border-radius: 10px;
    margin-top: calc(25% - 270px);
    padding: 70px 10px;
  }
  #idInputContainer,
  #passwordContainer {
    padding: 5px 30px;
  }
  #loginButton {
    margin-left: 32px;
    margin-right: 25px;
    background-color: aquamarine;
    border-radius: 12px;
    padding: 20px 0px;
    margin-top: 40px;
    color: white;
    font-size: large;
    font-weight: 700;
  }
  #idInput,
  #password {
    width: 100%;
    height: 55px;
    border-radius: 8px;
    font-size: large;
  }
  #password {
    margin-top: 0px;
  }
</style>
