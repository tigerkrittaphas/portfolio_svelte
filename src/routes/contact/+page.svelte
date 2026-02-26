<svelte:head>
  <title>Contact me</title>
</svelte:head>
<h1>Contact Me</h1>
    
    <form action="mailto:136419686+tigerkrittaphas@users.noreply.github.com" method="get">
        <label for="email">
            Email:
            <input id="email" name="email" type="email">
        </label>
        <label for="subject">
            Subject:
            <input id="subject" name="subject"  type="text">
        </label>
        <label for="body">
            Message:
            <textarea id="body" name="body"></textarea>
        </label>
        <button>Submit</button>
    </form>