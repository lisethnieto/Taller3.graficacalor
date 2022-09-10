# Taller3.graficacalor
import matplotlib.pyplot as plt
import matplotlib.cm as cm
from matplotlib.colors import LogNorm
import numpy as np
x, y = np.random.rand(10), np.random.rand(10)
z = (np.random.rand(9000000)+np.linspace(0,1, 9000000)).reshape(3000, 3000)
plt.imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.hot, norm=LogNorm())
plt.colorbar()
plt.show()

fig, ax = plt.subplots(5, 2, sharey = True)
ax[0, 0].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.hot, norm=LogNorm())
ax[1, 0].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.cool, norm=LogNorm())
ax[2, 0].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.hot, norm=LogNorm())
ax[3, 0].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.cool, norm=LogNorm())
ax[4, 0].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.hot, norm=LogNorm())
ax[1, 1].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.cool, norm=LogNorm())
ax[0, 1].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.hot, norm=LogNorm())
ax[2, 1].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.cool, norm=LogNorm())
ax[3, 1].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.hot, norm=LogNorm())
ax[4, 1].imshow(z+10, extent=(np.amin(x), np.amax(x), np.amin(y), np.amax(y)),
    cmap=cm.cool, norm=LogNorm())
