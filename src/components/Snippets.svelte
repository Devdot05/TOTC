<script lang="ts">
    type User = {
        name: String,
        age: Number,
        email: String
    }
    let users: User[] = [
        {
            name: "John Doe",
            age: 30,
            email: "john.doe@example.com"
        },
        {
            name: "Jane Smith",
            age: 25,
            email: "jane.smith@example.com"
        },
        {
            name: "Bob Johnson",
            age: 35,
            email: "bob.johnson@example.com"
        }
    ]
</script>

{#snippet userCard(user: User)}
    <section>
        <h3>name: {user.name}</h3>
        <p>age: {user.age}</p>
        <p>email: {user.email}</p>
    </section>
{/snippet}

{#each users as user}
   {@render userCard(user)}
{/each}

  