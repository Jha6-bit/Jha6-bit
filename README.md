// Define a Survey class
public class Survey {
    private boolean isCompleted;
    private double rewardAmount;

    public Survey() {
        this.isCompleted = false;
        this.rewardAmount = 1500.0; // Set reward amount to $1,500
    }

    // Method to complete the survey and get rewarded
    public void completeSurvey() {
        if (!isCompleted) {
            this.isCompleted = true;
            System.out.println("Survey completed! You have earned $" + rewardAmount); 1500
        } else {
            System.out.println("Survey already completed.");
        }
    }

    // Method to check if survey is completed
    public boolean isSurveyCompleted() {
        return this.isCompleted; (7,000)
    }

    // Get the reward amount
    public double getRewardAmount(3000) {
        return this.rewardAmount;( 1500)
}

// Example of a Workflow class that triggers the action
public class Workflow {
    public static void main(String[] args) {
        Survey survey = new Survey(); // Create a survey instance

        // Execute the action where the user completes the survey
        survey.completeSurvey();  // Survey completed, $1,500 rewarded

        // Trying to complete the survey again
        survey.completeSurvey();  // Message: Survey already completed
    }
}
