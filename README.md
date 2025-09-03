<div align="center">
  <a href="/README.md">English</a> | <a href="config/ZH_README.md">中文</a>
</div>

# Introduction to Iframe Generator
[Iframe Generator](https://iframe-generator.net/) is a free online tool designed specifically for web developers and content creators. It aims to simplify the process of creating iframe code, allowing users to quickly generate complete and usable HTML code without the need to memorize complex iframe attributes. Additionally, it supports saving and reusing configurations to meet various content embedding needs.


## Key Feature Highlights
1. **Comprehensive Attribute Coverage for Diverse Needs**  
The tool includes all standard and modern iframe attributes, such as src (the URL of the embedded content, the only required attribute), name (for link/form target positioning), title (accessibility description for screen readers), and allowfullscreen (supports full-screen display, suitable for videos/interactive content). It also covers dimension control (width/height, supporting units like pixels, percentages, vw/vh), behavior settings (scrolling to control scrollbars, loading to control loading timing), style definitions (directly configuring CSS styles like borders), and security-related attributes, ensuring the generated code complies with modern web standards.

2. **Real-Time Preview + Configuration Saving for Doubled Efficiency**  
- **Real-Time Preview**: After entering a valid source URL, the "Live Preview" function enables instant viewing of the iframe effect. It supports testing responsive performance (adapting to different screen sizes) without the need to repeatedly switch between code and preview pages.  
- **Configuration Saving**: It allows saving currently set iframe parameters (such as dimensions, security attributes, and functional permissions) locally. When the same configuration needs to be reused later, there’s no need to re-enter the parameters—simply load the saved configuration to quickly generate code. This is especially suitable for scenarios where fixed embedding rules are frequently used (e.g., uniformly styled video embedding, standardized form embedding).

3. **Balanced Security and Performance**  
It comes with multiple built-in security features: restricting iframe content permissions via the sandbox attribute (e.g., allow-scripts for enabling JS execution, allow-forms for enabling form submission, which can be checked as needed); supporting the referrerpolicy attribute to control the sending of referrer information during requests (e.g., "strict-origin-when-cross-origin" to ensure cross-origin security); and allowing configuration of Content Security Policy (CSP) to define resource loading rules and prevent security vulnerabilities. Meanwhile, it supports lazy loading with loading="lazy" to optimize page performance and reduce initial loading pressure.

4. **Ready-to-Use Code for Production Environments**  
The generated code is clean and optimized, requiring no additional modifications before being directly used in production environments. It is compatible with all modern browsers, ensuring consistent performance of embedded content across different devices.

## Preview
<div align="center">
  [![Iframe Generator](/website.png)
</div>

## Operation Process (3 Steps, Supporting Saving and Reuse)
1. **Configure Iframe Parameters**  
- Enter the URL of the content to be embedded (src attribute);  
- Set dimensions (width/height), scrollbars (scrolling), and border styles;  
- Configure security attributes (sandbox, referrerpolicy, CSP) and functional permissions (allow attribute, such as access permissions for cameras, microphones, and geolocation) as needed.

2. **Generate, Preview, and Save (Optional)**  
- Click the generate button: the tool automatically generates complete HTML code, and at the same time displays the actual effect in the preview area. You can adjust parameters in real time and view changes;  
- If you need to reuse the current configuration later, click the "Save Configuration" button to store the parameters locally (usually in the form of browser local storage or configuration files) to avoid repeated settings.

3. **Copy for Use or Load Historical Configurations**  
- After confirming the effect is correct, directly copy the generated code and paste it into the target web page to complete the embedding;  
- Next time you use it, click "Load Saved Configurations", select the historical parameters, and the tool will automatically fill in all settings to quickly generate new code.


## Common Use Cases
- **Website and Application Embedding**: Embed external websites, forms, and third-party applications to achieve content integration (e.g., multi-site dashboards, content previews). Saving fixed configurations can improve the efficiency of batch embedding;  
- **Media Embedding**: Generate iframe code for video platforms such as YouTube and Vimeo. It supports responsive design to adapt to mobile devices, and saving unified dimension configurations can ensure consistent page styles;  
- **Map Integration**: Create embedding code for map services like Google Maps and OpenStreetMap to display geographic location information. Saving embedding parameters for frequently used locations makes subsequent calls more convenient;  
- **Social Component Embedding**: Generate iframe code for social media feeds, posts, and widgets to achieve seamless integration. Saving standard configurations can reduce repeated operations.


## Additional Advantages
- **Accessibility-Friendly**: It automatically prompts users to add title attributes and ARIA labels, ensuring embedded content is compatible with screen readers and complies with accessibility standards;  
- **Free and Unrestricted**: It is completely free to use with no feature limitations or restrictions on the number of generations. It supports unlimited configuration saving and iframe code creation;  
- **Supporting Guides**: It provides rich and practical additional resources, such as tutorials on iframe loading event handling, web framework construction (replacing deprecated HTML frames), and WordPress site embedding, to help users solve advanced problems.


## Best Practice Recommendations
- **Performance Optimization**: Use lazy loading for iframes at the bottom of the page; set dimensions appropriately to avoid layout shifts; monitor the impact of iframes on the performance of the main page;  
- **Accessibility Adaptation**: Be sure to fill in meaningful title attributes; ensure content within iframes supports keyboard navigation; provide alternative content for screen readers;  
- **Security Configuration**: Minimize sandbox permissions based on the needs of the embedded content to avoid excessive access; set referrerpolicy and CSP appropriately in cross-origin scenarios to reduce security risks;  
- **Configuration Management**: Classify and save configurations for different embedding needs (e.g., videos, maps, forms), and name them clearly (e.g., "YouTube Video - 16:9 Responsive") to facilitate quick searching and reuse later.