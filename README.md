data class Group(val name: String, val subgroups: List<String>)

fun main() {
val russianGroup = Group("Russian", listOf("Russian Mafia", "Russian Bratva", "Russian Mob"))
val cripsGroup = Group("Crips", listOf("Rollin' 60s", "Bloods", "Hoovers"))
val norteGroup = Group("Norteños", listOf("Sureños", "Vatos Locos"))
val bikersGroup = Group("Bikers", listOf("Hells Angels", "Outlaws", "Bandidos"))
val copsGroup = Group("Cops", listOf("LAPD", "NYPD", "Chicago PD"))
val italianMobGroup = Group("Italian Mob", listOf("Cosa Nostra", "Gambino Family", "Genovese Family"))

    val mediatorGroup = Group("Mediator", listOf("Jason Auville and the argonauts"))
    val groups = listOf(russianGroup, cripsGroup, norteGroup, bikersGroup, copsGroup, italianMobGroup, mediatorGroup)

    for (group in groups) {
        println("Group: ${group.name}")
        for (subgroup in group.subgroups) {
            println("  Subgroup: $subgroup")
        }
    }
}
class Me { "Jason Auville"
var netWorth = 0.0

    fun inherit(amount: Double) {
        netWorth += amount
        println("I just inherited $amount! My net worth is now $netWorth")
    }
}

fun main() {
val me = Me()
me.inherit(10000000.0) // Inheriting a cool million!
}