# Las Semánticas de la Aplicación Crean la Brecha Semántica

Por supuesto, las restricciones de Collection+JSON no cubren todos los aspectos. Collection+JSON no especifica que los elementos en una colección deban ser publicaciones de microblog con un campo date_posted (fecha de publicación) y text (texto). Esa parte la inventé yo, porque quise diseñar un ejemplo simple de microblogging para este libro. Si hubiera optado por un ejemplo de "libro de recetas", aún podría usar Collection+JSON, pero los elementos tendrían campos de datos como ingredients (ingredientes) y preparation_time (tiempo de preparación).

Voy a llamar a estos elementos adicionales de diseño las semánticas de la aplicación (application semantics), porque varían de una aplicación a otra. Las semánticas de la aplicación son la causa de la brecha semántica mencionada en el **Capítulo 1**.

Si estuviera diseñando una API real de microblogging, probablemente definiría semánticas de aplicación más complejas que solo text y date_posted. Esto, en sí mismo, está bien. Pero actualmente, hay docenas de compañías diseñando APIs de microblogging, cada una con semánticas de aplicación distintas e incompatibles entre sí, lo que crea docenas de brechas semánticas distintas. Todas estas empresas están resolviendo el mismo problema de diferentes maneras, lo que obliga a sus usuarios a escribir clientes de software diferentes para realizar la misma tarea.

El hecho de que Collection+JSON no resuelva este problema no significa que no tenga sentido usarlo. La compatibilidad es una cuestión de grados. Dimos un gran paso hacia la compatibilidad en los años 90 cuando dejamos de inventar protocolos de Internet personalizados y estandarizamos en HTTP. Si todos acordáramos servir documentos JSON, eso tal vez no sería una solución técnicamente perfecta, pero reduciría la brecha semántica. Estandarizar en Collection+JSON la reduciría aún más.

Si los publicadores de APIs de microblogging se reunieran y acordaran usar un conjunto común de semánticas de aplicación, la brecha semántica en el microblogging desaparecería casi por completo. (Esto sería un perfil, y cubriré esta idea en el **Capítulo 8**). Cuantas más restricciones compartamos y más compatibles sean nuestros diseños, más pequeña será la brecha semántica y más se beneficiarán nuestros usuarios. 

Quizás no quieras que tu API sea interoperable con la de tus competidores, pero hay mejores formas de diferenciarse que ampliando artificialmente la brecha semántica. Mi objetivo con este libro es que te enfoques en las partes de tu API que realmente ofrecen algo nuevo, en los puntos donde existe una brecha semántica porque nadie más ha seguido ese camino antes.

   #### Application Semantics Create the Semantic Gap | 27 y 28
