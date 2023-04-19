1. q0: Read the first symbol.
   - If 'a', replace with 'a'', move right, and transition to q1.
   - If not 'a', reject (move to the reject state, qR).

2. q1: Look for the first unmarked 'b'.
   - If 'b', move right, and transition to q2 (mark the 'b' as 'b'').
   - If 'a', 'a'', 'a+', 'b'', or '$', move right and stay in q1.
   - If 'blank', move left and transition to q2.

3. q2: Look for the first unmarked 'a' in the second half.
   - If 'a', move right, and transition to q3 (mark the 'a' as 'a+').
   - If 'a+', 'b', 'b'', or '$', move right and stay in q2.
   - If 'blank', move left and transition to q4.

4. q3: Move left to the beginning of the input.
   - If 'a+', 'a'', 'b'', 'b', or '$', move left and stay in q3.
   - When the leftmost symbol 'a'' is found, move right and transition to q1.

5. q4: Check for unmarked 'b's in the remaining input.
   - If 'b', move right and stay in q4.
   - If 'b'', move right and transition to q5.
   - If '$', move right and stay in q4.
   - If 'blank', move left and transition to q6.

6. q5: Look for unmarked 'a's in the second half.
   - If 'a', move right and stay in q5.
   - If 'a+', move right and stay in q5.
   - If 'b', 'b'', or '$', move right and stay in q5.
   - If 'blank', reject (move to the reject state, qR).

7. q6: Check for unmarked 'a's in the first half.
   - If 'a', reject (move to the reject state, qR).
   - If 'a'', move left and stay in q6.
   - If '$', move right and transition to q7.

8. q7: Replace marked 'a''s and 'a+'s with original 'a's.
   - If 'a'', replace with 'a', move right, and stay in q7.
   - If 'a+', replace with 'a', move right, and stay in q7.
   - If 'b'', move right and transition to q8.

9. q8: Replace marked 'b''s with original 'b's.
   - If 'b'', replace with 'b', move right, and stay in q8.
   - If 'blank', move left and transition to q9.

10. q9: Move left to the beginning of the input.
   - If 'a', 'b', or '$', move left and stay in q9.
   - If 'blank', move right and transition to q10.

11. q10: Move right to the end of the input.
   - If 'a', 'b', or '$', move right and stay in q10.
   - If 'blank', move left and transition to q11.

12. q11: Check if there are any unmarked 'a's left.
   - If 'a', reject (move to the reject state, qR).
   - If 'a+', accept (move to the
