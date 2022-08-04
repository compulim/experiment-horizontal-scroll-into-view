# experiment-horizontal-scroll-into-view

This is an experiment to see how different browsers scroll widgets into view.

Try the [live demo here](https://compulim.github.io/experiment-horizontal-scroll-into-view/).

## Experiment result

✔️ indicates browser will scroll widget into the view when focus by <kbd>TAB</kbd>.

❌ indicates browser will not scroll widget into the view when focus by <kbd>TAB</kbd>.

<table>
   <thead>
      <tr>
         <th>Widget</th>
         <th>Condition</th>
         <th>Chrome 103</th>
         <th>Edge 105</th>
         <th>Firefox 103</th>
         <th>Safari 15 (macOS)</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td rowspan="2"><code>&lt;button&gt;</code></td>
         <td>Partially on-screen</td>
         <th>❌</th>
         <th>❌</th>
         <th>❌</th>
         <th>❌</th>
      </tr>
      <tr>
         <td>Completely off-screen</td>
         <th>✔️</th>
         <th>✔️</th>
         <th>✔️</th>
         <th>✔️</th>
      </tr>
      <tr>
         <td rowspan="2"><code>&lt;input type="text"&gt;</code></td>
         <td>Partially on-screen</td>
         <th>✔️</th>
         <th>✔️</th>
         <th>❌</th>
         <th>❌</th>
      </tr>
      <tr>
         <td>Completely off-screen</td>
         <th>✔️</th>
         <th>✔️</th>
         <th>✔️</th>
         <th>✔️</th>
      </tr>
   </tbody>
</table>

> Note: For Safari, we use <kbd>OPTION</kbd> + <kbd>TAB</kbd> to focus on `<button>`.

## Conclusions

All modern browsers will scroll widgets into the view if they are completely off-screen.

However, when the widgets is a text box and is partially off-screen, Chrome and Edge will scroll them into the view. And Firefox and Safari will not.

## Recordings

### Edge 105

https://user-images.githubusercontent.com/1622400/182949928-59faae63-fa57-4e92-8616-67cc3d780879.mp4

### Firefox 103

https://user-images.githubusercontent.com/1622400/182951598-6f3c06dc-de8b-41d9-a31b-07a57162499b.mp4
