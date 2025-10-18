<script lang="ts">
    let count = $state(0);
    let name = $state("John");
    let firstName = $state("Dotun");
    let lastName = $state("Timothy");
    firstName = "Olawole";
    let fullName = $derived (firstName + " " + lastName);
    let quantity = $state(100);
    let price = $state(10);
    let total = $derived (quantity * price);
    let increment = () => count++;
    let decrement = () => count--;
    
</script>

<div class="col-6 p-3 shadow-sm mx-auto">
    <div class="mb-3">
        <p>{count}</p>
        <button onclick={increment} class="btn btn-primary">+</button>
        <button onclick={decrement} class="btn btn-success">-</button>
    </div>
    <div>
        <p>{name}</p>
        <input type="text" bind:value={name} class="form-control">
    </div>
    <div>
        <p>{fullName}</p>
        <input type="text" bind:value={firstName} class="form-control" placeholder="First Name">
        <input type="text" bind:value={lastName} class="form-control" placeholder="Last Name">
    </div>
    <div>
        <p>{total}</p>
        <input type="number" bind:value={quantity} class="form-control" placeholder="quantity">
        <input type="number" bind:value={price} class="form-control" placeholder="price">
    </div>
</div>
