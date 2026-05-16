package com.example.settings

/**
 * Configuration class representing the specific sensitivity and force settings 
 * for the touch panel interface.
 */
object TouchPanelSettings {

    /**
     * Represents the "Headshot Force" setting.
     * Original Requirement: Headshot Force 60% Touch Panel
     * 
     * Value is represented as a percentage (0.60f for 60%).
     */
    const val HEADSHOT_FORCE_PERCENTAGE: Float = 0.60f
    
    /**
     * Target component identifier.
     */
    const val TARGET_COMPONENT: String = "Touch Panel"

    /**
     * Function to retrieve the current configuration string for display purposes.
     * 
     * @return A formatted string of the current setting.
     */
    fun getConfigurationLabel(): String {
        return "Headshot Force ${ (HEADSHOT_FORCE_PERCENTAGE * 100).toInt() }% $TARGET_COMPONENT"
    }
}
