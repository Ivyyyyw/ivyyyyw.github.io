---
title: "Site Statistics"
date: 2024-10-18
draft: false
_build:
  list: never
menu: {}
search_exclude: true
noindex: true
---

<div style="max-width: 800px; margin: 0 auto; padding: 20px;">
  <h1 style="text-align: center; color: #1f2937; margin-bottom: 30px;">📊 Site Visitor Statistics</h1>
  
  <div style="background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%); 
              border: 1px solid #0ea5e9; 
              border-radius: 12px; 
              padding: 20px; 
              margin: 20px 0; 
              box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);">
    <p style="margin: 0; color: #0f172a; line-height: 1.6;">
      🌍 This page shows real-time visitor statistics and geographic distribution for the website. 
      The data helps understand audience reach and engagement patterns.
    </p>
  </div>
  
  <!-- MapMyVisitors Widget Container -->
  <div id="visitor-map-container" style="margin: 30px 0; text-align: center;">
    <h2 style="color: #374151; margin-bottom: 20px;">🗺️ Visitor Map</h2>
    
    <!-- The map will be inserted here by the script -->
    <div id="map-placeholder" style="min-height: 400px; 
                                     background: #f8fafc; 
                                     border: 2px dashed #cbd5e1; 
                                     border-radius: 8px; 
                                     display: flex; 
                                     align-items: center; 
                                     justify-content: center; 
                                     color: #64748b;">
      <p>📍 Loading visitor map...</p>
    </div>
  </div>
  
  <div style="text-align: center; margin-top: 40px; padding-top: 20px; border-top: 1px solid #e5e7eb;">
    <p style="color: #6b7280; font-size: 14px;">
      🔒 This page is not indexed by search engines and is for analytics purposes only.
    </p>
  </div>
</div>

<!-- MapMyVisitors Script -->
<script id="mapmyvisitors" type="text/javascript"
        src="//mapmyvisitors.com/map.js?d=GIGVYtMFETiplLXRv1J3KrX-flUxOvIow62-A39cMqQ&cl=ffffff&w=a"></script>

<script>
// Wait for the map to load and then move it to our container
document.addEventListener('DOMContentLoaded', function() {
  setTimeout(function() {
    // Find the MapMyVisitors element and move it to our container
    const mapElements = document.querySelectorAll('[id*="mapmyvisitors"], [class*="mapmyvisitors"]');
    const container = document.getElementById('map-placeholder');
    
    if (mapElements.length > 0 && container) {
      // Clear the placeholder
      container.innerHTML = '';
      container.style.background = 'transparent';
      container.style.border = 'none';
      
      // Move the map to our container
      mapElements.forEach(element => {
        container.appendChild(element);
      });
    }
  }, 2000); // Wait 2 seconds for the map to load
});
</script>
