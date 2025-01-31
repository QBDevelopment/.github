# Quartz
# Blockchain
# Development

![QBD](./qbd.jpg)


<h1>Rust Code Style Guide</h1>

<h2>1. Formatting</h2>
<p>All Rust code must be formatted using <code>nightly rustfmt</code>. To apply formatting, run:</p>
<pre><code>cargo +nightly fmt</code></pre>

<h2>2. Naming Conventions</h2>
<ul>
    <li>Variable, function, and method names must reflect their purpose.</li>
 <li>Use descriptive names: 
        <ul>
            <li><code>create_user_handler</code> - OK</li>
            <li><code>create_user_service</code> - OK</li>
            <li><code>create</code> - NO</li>
            <li><code>create_user</code> - NO</li>
        </ul>
    </li>
    <li>Follow Rust's snake_case convention for variables and functions.</li>
    <li>Structs and enums should use PascalCase (e.g., <code>TransactionStatus</code>).</li>
    <li>Constants should be in SCREAMING_SNAKE_CASE.</li>
</ul>

<h2>3. Code Quality</h2>
<ul>
    <li>Write clean and maintainable code.</li>
    <li>Avoid unnecessary complexity.</li>
    <li>Avoid unnecessary <code>unwrap()</code> and <code>clone()</code>.</li>
    <li>Minimize global states and side effects.</li>
    <li>Using <code>::</code> only in imports!</li>
</ul>

<h2>4. Branch Management</h2>
<ul>
    <li>After merging a Pull Request, delete the intermediate branch.</li>
    <li>Keep the main branch clean and production-ready.</li>
</ul>

<h2>5. Best Practices</h2>
<ul>
    <li>Use <code>clippy</code> for linting: <pre><code>cargo clippy</code></pre></li>
    <!-- <li>Write unit tests for all critical functions.</li> -->
    <li>Handle errors gracefully using <code>Result</code> and <code>Option</code>.</li>
    <li>Avoid unnecessary panics.</li>
</ul>

<h2>6. GitHub Projects and Weekly Reports</h2>
<ul>
    <li>Use GitHub Projects to track tasks and milestones.</li>
    <li>Each task should have a clear description, priority, and assignee.</li>
    <li>Weekly reports must be submitted between Friday and Sunday.
        <a href="https://docs.google.com/forms/d/e/1FAIpQLScZOcUixej1cyRtmf1CC264Ylfk7tRHIGu-7Xq-9-X9TkfkxQ/viewform">Send weekly report</a>
    </li>
    <li>The report should include completed tasks, ongoing work, and blockers.</li>
</ul>

<p>Following these guidelines ensures high-quality, maintainable, and scalable Rust code.</p>
