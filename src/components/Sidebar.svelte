<script lang="ts">
    // export let name: string;
    // export let age: number
    // const {name, age, location, hubby} = $props()
    const {children} = $props()
</script>
<aside class="bg-warning">
    <!-- <h3>This is Child component</h3>
    <p>name:{name}</p>
    <p>age: {age}</p>
    <p>age: {location}</p>
    <p>age: {hubby}</p> -->

    <!---Children's props-->
    <!---How to pass in HTML content from parent to child-->

    <section>
        {@render children()}
    </section>

</aside>