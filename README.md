<!-- This is the solution of TwoSum  -->

 for(int i=0; i<nums.length;i++){<br>
            for(int j=i+1; j<nums.length; j++){<br>
                int comp = target - nums[i];

                if(nums[j] == comp){
                    return new int[] {i,j};
                }
            }
        }
        throw new  IllegalArgumentException("no match found");
