<template>
    <div class="">
        <form action="action_page.php" method="post">


            <div class="container">
                <label for="uname"><b>Username</b></label>
                <input type="text" placeholder="Enter Username" name="uname" required>

                <label for="psw"><b>Password</b></label>
                <input type="password" placeholder="Enter Password" name="psw" required>

                <button type="submit">Login</button>
                <label>
                <input type="checkbox" checked="checked" name="remember"> Remember me
                </label>
            </div>

            <div class="container" style="background-color:#f1f1f1">
                <div class="container2">hello</div>
                <button type="button" class="cancelbtn">Cancel</button>
                <span class="psw">Forgot <a href="#">password?</a></span>
            </div>
        </form>
    </div>
</template>

<script>

export default {
  name: 'Practice1',
}
</script>

<style lang="sass">
$breakpoint: 300px;
$border-config: 3px solid #f1f1f1

%default-config
    width: 100%
    padding: 12px 20px
    margin: 8px 0
    display: inline-block
    border: 1px solid #ccc
    box-sizing: border-box

form
    border: $border-config

input[type=text], input[type=password] 
    @extend %default-config

button 
    background-color: #04AA6D
    color: white
    padding: 14px 20px
    margin: 8px 0
    border: none
    cursor: pointer
    width: 100%

button:hover 
    opacity: 0.8

.cancelbtn 
    width: auto
    padding: 10px 18px
    background-color: #f44336


.container 
    padding: 16px
    .container2
        color: blue
        margin: 8px 0


span.psw 
    float: right;
    padding-top: 16px;

@media (max-width: $breakpoint) 
    span.psw 
        display: block
        float: none
  
    .cancelbtn 
        width: 100%

</style>