# NZ public holiday entries for Emacs Calendar

Remove default holidays, then append NZ calendar by adding this to your init.el:


```;; remove unnecessary calendars and replace with one localised to NZ
   (setq holiday-general-holidays nil) 
   (setq holiday-christian-holidays nil)
   (setq holiday-hebrew-holidays nil)
   (setq holiday-islamic-holidays nil)
   (setq holiday-bahai-holidays nil)
   (setq holiday-oriental-holidays nil)

   (setq calendar-holidays (append calendar-holidays holiday-nz-holidays))
   
```