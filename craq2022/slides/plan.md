## Plan

### Imaging and interferometry

(could be shorter to benefit kernel phase, but maybe would loose people by
skipping steps)

- Imaging and challenges (diffraction limited, bright star, even if had planet, hard to see)
- Why does it work?
- When get image from star with telescope, see psf. This contains info about
  spatial frequency distribution of info (shown on the right)
- Smaller aperture -> Smaller frequency coverage -> Bigger diffraction limit
- This is all for single hole, but can also play this game with more than one
  hole (or one than more telescope)
- Add hole to add sine wave pattern
- Longer distance to get finer sampling in PSF and better fourier coverage
- Even if holes (or telescopes) are small, can get long distance between two and
  have resolution (lambda / Dx)
- But limited in direction and info content by fact that two small holes instead
  of one big, like saw before: can add more. Third one gives two new directions
  to cover

### AMI
- This is principle that AMI uses: light passes through seven hole and the image
  is interference pattern from 7 holes
- But limited to 1 telescope so here don't boost diameter: what's the point?
  (Appart from blocking light, which generally does not help)
- High pass fitler: keep light from specific holes, core becomes smaller than
  diffcation peak: finer scales
- Most importantly: Mask is non-redundant, so can isolate where fourier info
  comes from. Each splodge is from 1 baseline
- Each peak has fourier phase associated: Phase is info from object along with
  errors from both apertures
- Idea is to use closure phase: self-calibrating against errors

- Applications with NIRISS: planets and disks
- Talk about GTO planets

### Kernel
- Kernel is basically generalizing AMI to full pupil, using the fact that WFE
  are small
- true for jwst
- Get the benefit (most) without loosing light
- Brown dwarfs
- Slide on GO program?
