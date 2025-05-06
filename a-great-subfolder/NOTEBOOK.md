# This is SHOWCASE.ipynb

```python
import matplotlib.pyplot as plt
import numpy as np

print("This is a simple script to plot a sine wave.")
```

    This is a simple script to plot a sine wave.


## Voltage Curve

some experiments.

```python
t = np.arange(0.0, 2.0, 0.01)
s = 1 + np.sin(2*np.pi*t)
plt.plot(t, s)

plt.xlabel('time (s)')
plt.ylabel('voltage (mV)')
plt.title('About as simple as it gets, folks')
plt.grid(True)
plt.show()

```


    
![png](NOTEBOOK_files/NOTEBOOK_3_0.png)
    


<div style="text-align: center; margin-left: 45%;">
    <a href="https://github.com" target="_blank" style="text-decoration: none;">
        <button style="background-color: #0366d6; color: white; border: none; padding: 10px 20px; font-size: 16px; display: flex; align-items: center; cursor: pointer;">
            <img src="/contents/github-logo.svg" alt="GitHub Logo" style="width: 20px; height: 20px; margin-right: 10px;">
            GITHUB CODE
        </button>
    </a>
</div>

<a href="contents/sample.mp4" target="_blank">Click here to view the video from anchor tag.</a>
# Sample Video
<video width="1280" height="720" controls>
    <source src="contents/sample.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
