<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<style>
  body {
    width: 300px;
    font-family: -apple-system, Arial, sans-serif;
    padding: 12px;
    margin: 0;
    background: #202124;
    color: #e8eaed;
  }
  h1 {
    font-size: 14px;
    font-weight: 600;
    margin: 0 0 10px 0;
  }
  input {
    width: 100%;
    box-sizing: border-box;
    padding: 8px;
    border-radius: 6px;
    border: 1px solid #5f6368;
    background: #303134;
    color: #e8eaed;
    font-size: 14px;
    margin-bottom: 8px;
  }
  .row {
    display: flex;
    gap: 6px;
    margin-bottom: 10px;
  }
  button {
    padding: 8px 10px;
    border: none;
    border-radius: 6px;
    font-weight: 600;
    font-size: 13px;
    cursor: pointer;
  }
  #openBtn {
    flex: 1;
    background: #8ab4f8;
    color: #202124;
  }
  #openBtn:hover { background: #aecbfa; }
  #saveBtn {
    background: #3c4043;
    color: #e8eaed;
  }
  #saveBtn:hover { background: #4a4d51; }
  h2 {
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 0.04em;
    color: #9aa0a6;
    margin: 12px 0 6px 0;
  }
  .fav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 6px 8px;
    border-radius: 6px;
    background: #303134;
    margin-bottom: 4px;
    font-size: 13px;
  }
  .fav span {
    cursor: pointer;
    flex: 1;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .fav .remove {
    color: #9aa0a6;
    cursor: pointer;
    padding: 0 4px;
    font-size: 14px;
  }
  .fav .remove:hover { color: #f28b82; }
  #empty {
    font-size: 12px;
    color: #9aa0a6;
    padding: 4px 0;
  }
</style>
</head>
<body>
  <h1>Quick Open</h1>
  <input type="text" id="site" placeholder="e.g. github.com or a search term">
  <div class="row">
    <button id="openBtn">Open</button>
    <button id="saveBtn" title="Save as favorite">★ Save</button>
  </div>
  <h2>Favorites</h2>
  <div id="favorites"></div>
  <script src="popup.js"></script>
</body>
</html>
