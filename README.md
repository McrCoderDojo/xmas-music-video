# Manchester Coder Dojo Christmas Music Video


    samps = "c:\\samples**"
    use_bpm 100

    live_loop :bar do
      sleep 4
    end
    
    
    live_loop :habanera do
      use_synth :fm
      use_transpose 0
      play (ring :d, :r, :r, :a, :f5, :r, :a, :r).tick
      sleep 0.25
    end
    
    live_loop :drums do
      sample :bd_haus, cutoff: 110
      synth :beep, note: 49, attack: 0,
        release: 0.1
      sleep 0.5
    end
    
    live_loop :samp do
      sync :bar
      #sample samps, "cavalry-brass-fanfare", amp: 8
      sleep 8
    end
    
