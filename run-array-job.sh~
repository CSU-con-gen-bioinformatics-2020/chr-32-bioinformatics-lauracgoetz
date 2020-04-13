#!/bin/bash

#SBATCH --time=02:00:00
#SBATCH --output=run-array-out-%A_%a
#SBATCH --error=run-array-error-%A_%a
#SBATCH --mail-type=ALL
#SBATCH --mail-user=user@email.edu
#SBATCH --array=1-9


./map-N-files-from-K.sh 128 $((SLURM_ARRAY_TASK_ID * 128 + 1))
