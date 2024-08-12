<p><strong>Development Notice:</strong> This Repository is under construction. Content may not work, exist, or may change.</p>

<h2>RodentSociety-Repo</h2>
<p style="color: grey;">
    <i>This repository serves as a centralized place to find resources and showcase ongoing projects.</i>
</p>

<h4>Content Table</h4>
<blockquote>
    <h4>Projects</h4>
    <a href="#ProjectKoda">Project Koda</a>: Open Source AI Initiative<br>
    <a href="#ProjectHoney">Project Honey</a>: SqueakSecure 2.0 with a honeypot redirector<br>
    <h4>Resources</h4>
    <a href="/templates">Collection of Free Templates</a><br>
    <h4>Tools</h4>
    <a href="#RsLogMod">RsLogMod</a>: Python logging module<br>
    <h5>Changelog</h5>  
    <ul>
        <li>Aug 12th: <strong>[Release]</strong><a href="#RsLogMod"> RsLogMod</a>: released on pypi<br><br></li>
        <li>Aug 5th: <strong>[Added]</strong> project information for <a href="#ProjectKoda">Project Koda</a>: Open Source AI Initiative<br><br></li>
    </ul>
</blockquote>
<br>
<hr>
<h4>Contribution & How to Get in Touch</h4>
<p>
    <i>If you have any suggestions or improvements, you can make a pull request, open an issue, or pitch it directly.</i>
</p>
<p>
    <i>If you have any questions or just want to chat, there are several ways to get in touch if GitHub doesn't cut it:</i>
</p>
<ul>
    <li>Discord: l.l.l.lllll.llll.lll.l.l.lll.l.l</li>
    <li>Reddit: <a href="https://www.reddit.com/u/Rodent_Dex/">Rodent_Dex</a></li>
</ul>

<h4>License Information</h4>
<p>
    This repository contains various types of content, each governed by different licenses. Please refer to the information provided in the individual subdirectories or file header text.
</p>

<h3 id="ProjectKoda">Project Koda</h3>
<p>Project Koda is an open-source AI initiative designed to be a versatile companion in cybersecurity and more. It blends technical support with engaging conversation, offering users both expertise and friendly interaction.</p>

<h4>Key Features</h4>
<ul>
    <li><strong>Conversational Style</strong>: Adapts to formal, informal, or technical discussions.</li>
    <li><strong>Expertise Areas</strong>: Cybersecurity, programming, and casual topics.</li>
    <li><strong>Emotional Support</strong>: Provides companionship as an added benefit.</li>
</ul>

<h4>Technical Highlights</h4>
<ul>
    <li><strong>Model Architecture</strong>: Transformer-based for advanced natural language processing.</li>
    <li><strong>Programming Languages</strong>: Python & C.</li>
</ul>

<h4>Datasets</h4>
<ul>
    <li><strong>Common Vulnerabilities & Exploits Data (1999 - 2024)</strong></li>
    <li><strong>Books for Vocabulary Building and Contextual Understanding</strong></li>
    <li><strong>Programming Language Documentation</strong></li>
</ul>

<h4>Learn More</h4>
<p>Discover the potential of Koda and its integration with our other projects:</p>
<ul>
    <li><strong>Project Honey</strong>: An extension to a mousetrap-based intrusion prevention system for counterintelligence.</li>
    <li><strong>Project RodentEye</strong>: An OCR-based monitoring program for intelligence gathering.</li>
</ul>
<hr>

<h3 id="RsLogMod">RsLogMod</h3>

<p><strong>RsLogMod</strong> is a Python logging module that helps manage log files with features like log rotation, custom log paths, and log levels. It's designed to be simple to use and configure, emphasizing flexibility.</p>

<h4>Installation</h4>
<p>To install the module, use pip:</p>

<pre><code>pip install rslogmod</code></pre>

<h4>Getting Started</h4>
<p>Here’s a quick example to get you logging:</p>

<pre><code>from RsLogMod import rlog

# Log a simple message
rlog(log_name='my_log', log_level=1, log_entry='This is a log entry.')

# Example output: [INFO] 2024-12-02 13:20: This is a log entry.
</code></pre>

<h5>Explanation</h5>
<ul>
    <li><strong>log_name</strong>: The name of the log file (e.g., <code>my_log</code>).</li>
    <li><strong>log_level</strong>: The log level, where <code>1</code> typically corresponds to <code>INFO</code>.</li>
    <li><strong>log_entry</strong>: The message you want to log.</li>
</ul>

<p>This will create a log file named <code>my_log.log</code> (if it doesn't already exist) in the configured directory with the entry formatted as shown above.</p>

<h4>Log Levels & Prefixes</h4>
<p>RsLogMod supports several log levels, each with its own prefix:</p>
<ul>
    <li><strong>0</strong>: <code>[DEBUG]</code> - For detailed debugging information.</li>
    <li><strong>1</strong>: <code>[INFO]</code> - For general information about program execution.</li>
    <li><strong>2</strong>: <code>[ERROR]</code> - For errors that occur during execution.</li>
    <li><strong>3</strong>: <code>[CRITICAL]</code> - For critical issues that need immediate attention.</li>
    <li><strong>4</strong>: <code>[SEC-ALERT]</code> - For security-related alerts.</li>
    <li><strong>5</strong>: <code>[SEC-BREACH]</code> - For security breaches or serious security issues.</li>
</ul>

<h4>Customization</h4>
<p>To customize how RsLogMod operates, such as changing the log file directory, setting the maximum log file size, or enabling log rotation, you can use the <code>RsManager</code> class.</p>

<h5>Using RsManager</h5>
<p>Here's how you can customize various settings:</p>

<h6>Set Log Folder Path</h6>

<pre><code>from RsLogMod import RsManager

# Create an RsManager instance
manager = RsManager()

# Set a new log folder path
manager.log_folder_path('/new/log/directory')

# Display the current configuration to verify changes
manager.display()
</code></pre>

<h6>Set Maximum Log Size</h6>

<pre><code>from RsLogMod import RsManager

# Create an RsManager instance
manager = RsManager()

# Set the max size for log files to 20 MB
manager.log_max_size(20)

# Display the current configuration to verify changes
manager.display()
</code></pre>

<h6>Enable or Disable Log Rotation</h6>

<pre><code>from RsLogMod import RsManager

# Create an RsManager instance
manager = RsManager()

# Enable log rotation
manager.log_rotation(True)

# Display the current configuration to verify changes
manager.display()
</code></pre>

<h5>Explanation</h5>
<ul>
    <li><strong>RsManager</strong>: This class handles the configuration settings for RsLogMod, such as where log files are stored, how large they can grow before being rotated, and whether log rotation is enabled.</li>
    <li><strong>log_folder_path(path: str)</strong>: Sets the directory where logs are saved.</li>
    <li><strong>log_max_size(mega_bytes: int)</strong>: Sets the maximum size for log files in megabytes.</li>
    <li><strong>log_rotation(value: bool)</strong>: Enables or disables log rotation.</li>
</ul>

<h4>Configuration</h4>
<p>RsLogMod uses a <code>configs.json</code> file for settings. Here’s an example:</p>

<pre><code>{
    "log_rotation": false,
    "max_size_in_mega_bytes": 10,
    "out_dir": "/path/to/logs"
}
</code></pre>

<ul>
    <li><strong>log_rotation</strong>: Enable or disable log rotation.</li>
    <li><strong>max_size_in_mega_bytes</strong>: The maximum size of a log file before it is rotated.</li>
    <li><strong>out_dir</strong>: The directory where log files will be stored.</li>
</ul>

<p>You can update these settings programmatically using the <code>RsManager</code> class, as shown in the examples above.</p>

<h4>License</h4>
<p>This project is licensed under the <a href="https://github.com/D-3-X/Rodent-REPO/blob/main/licenses/MIT_License.txt">MIT License</a>. See the LICENSE file for details.</p>
