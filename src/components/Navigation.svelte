<script>
    import Sidebar from "./Sidebar.svelte";
</script>
<div class="bg-primary">
    this is parent component
    <!-- <Sidebar name="John" age={22} location="Nigeria" hubby="coding"/> -->

     <!---Children's props-->
    <!---How to pass in HTML content from parent to child-->

    <Sidebar>
        <h1>Hello World</h1>
        <ul>
            <li>About</li>
            <li>Services</li>
            <li>Contact</li>
        </ul>
         
    </Sidebar>
</div>