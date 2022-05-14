# some best ways to optimize your website for better lighthouse scorew
The most critical CSS styling is loaded and applied as soon as possible with either an intentionally render blocking conventional reference to a very small CSS file (<10KB) or with a non-render blocking inline <style> block embedded directly in the HTML
  
  `<link rel="stylesheet" media="print" onload="this.onload=null;this.removeAttribute('media');" href="non-critical.css">`
