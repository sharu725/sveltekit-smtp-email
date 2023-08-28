<script>
    export let form;
</script>

<div class="wrapper">
    <fieldset>
        <legend>Send Emails</legend>
        <form method="POST" class="container">
            <div class="input">
                <label for="">To:</label>
                <input name="to" type="email" value="sharath.dt@gmail.com" />
            </div>
            <div class="input">
                <label for="">Subject:</label>
                <input name="subject" type="text" value="A test subject" />
            </div>
            <div class="input">
                <label for="">Body:</label>
                <textarea name="body" rows="6" value="A test message" />
            </div>
            <button type="submit">Send</button>
        </form>
        <p class="success">{form?.success || ""}</p>
    </fieldset>
</div>

<style>
    .wrapper {
        max-width: 800px;
        margin: 2em auto;
    }
    fieldset {
        padding: 2em;
        box-shadow: 0 10px 15px -3px #0000001a, 0 4px 6px -4px #0000001a;
    }
    legend {
        font-weight: bold;
        font-size: 2em;
        padding: 0 0.25em;
        color: #333;
    }
    .container {
        max-width: 400px;
    }
    .input {
        display: grid;
        margin-bottom: 1.5em;
    }
    label {
        font-weight: 600;
        margin-bottom: 0.25em;
        color: #555;
    }
    input {
        padding: 5px;
    }
    button {
        cursor: pointer;
        padding: 0.5em 1em;
        border-radius: 4px;
        border: 1px solid darkseagreen;
        background-color: darkseagreen;
    }
    .success {
        color: #0a5;
    }
</style>
