# MIDAS-task-2

### Requirements 

`pip install -r requirements.txt`

* Preferably use Google Colabotory to get all the dependancies pre installed.


### Task submission Repository

* For all the Initial experiment, conducted before proceeeding to the task cann be found in  MIDAS__Task2__Initial__experiments.ipynb
* The notebook pertaining to 1st part is MIDAS_Task2_Part1.ipynb
* The notebook pertaining to 2nd part is MIDAS_Task2_part2.ipynb
* The notebook pertaining to 3rd part is MIDAS_Task2_part3.ipynb
* For the summary of the results are in Results_Summary.ipynb

### Instruction regrading run functions
 
 * def run(model,criterion,optimizer,scheduler,load_dir,load_model,load_epch=0,N_EPOCHS=20,save_fq=5,load=False,ch=3):
 * def run_pre(model,criterion,optimizer,scheduler,load_dir,load_model,load_epch=0,N_EPOCHS=20,save_fq=5,load=False,ch=3):
 * def run_train(model,criterion,optimizer,scheduler,load_dir,load_model,load_epch=0,N_EPOCHS=20,save_fq=5,load=False):
 
   *Parameters*:
   
   model- pytorch based deep learning model object
   
   criterion- loss function
   
   optimizer- optimizer object
   
   scheduler- scheduler object
   
   load_dir- path for the load root where the model would be saved/loaded
   
   load_model- name of subdirectory where the model would be saved/loaded
   
   load_epoch- epoch number when model checkpoint is pre-loaded
   
   N_EPOCHS- number of epochs to be trained and evaluated in the current run
   
   save_fs- save frequency of the model checkpoint while training
   
   load- if True load pre saved checkpoint , if False train from scratch.
   
   ch- The number of channels of image in the dataset for training and evaluated
   
   
   
## Instruction regrading  load checkpoint
   
   def load_checkpoint(model, save_folder, model_name,epoch,opt,device ,best_model=False)
   
   *Parameters*:
   
    model- pytorch based deep learning model object
    
    save_folder- path for the load root where the model would be loaded
   
    model_name- name of subdirectory where the model would be loaded
   
    epoch- epoch number when model checkpoint is pre-loaded
    
    opt-optimizer object
    
    device- 'cpu' or 'cuda'
    
    best_model- if True loads best model
    
   *Return*:
   
   model, opt, epoch, time1
   
   model- loaded model
   
   opt- optimizer with upadted parameters from chckpoint
    
   epoch- last trained epoch
   
   time1- time taken till training the checkpoint.
   
   
   *All the checkpoints are  present in the link*- [here](https://drive.google.com/drive/folders/1Hppdc1RmkHPDJUg1V5OYASSe-JHe1lYs?usp=sharing)

   
