# AI Video on Grace Hopper

Algorithm used to create a 65 second AI video about Grace Hopper (compiler pioneer, COBOL).

**Tools:** DigEn AI (video clips), CapCut (editing)

## Algorithm 1: Compiler (A-0 style, Grace Hopper's idea)

```
START
  read the program (list of subroutine numbers with values)
  output <- empty
  FOR each instruction in the program DO
      code <- find subroutine (instruction.number) in library
      put instruction.values into code
      add code to output
  END FOR
  save output as machine code
END
```

## Algorithm 2: Video making process

```
START
  scientist <- "Grace Hopper"
  research life and work (compiler, COBOL)
  prepare reference image (Grace on left, student on right)
  divide video into 13 scenes, each 5 seconds
  write prompt and short dialogue for each scene

  i <- 1
  WHILE i <= 13 DO
      clip <- generate scene i in DigEn AI using prompt[i] and reference image
      IF clip is not good (face/dress changed or lip-sync wrong) THEN
          edit prompt[i]
          GOTO generate again
      END IF
      save clip
      i <- i + 1
  END WHILE

  import all 13 clips into CapCut
  arrange clips in scene order
  add transitions and background music
  export final video (13 x 5 = 65 seconds)
END
```

## Files

- `grace_hopper_report.pdf` : description, flowchart and scene-wise dialogues
- Final video: `GraceHopper.mp4`
