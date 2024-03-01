# CheatSheet-JSON
para el mapa
public Iterator getIterator()
{
  return mapa.entrySet().iterator();
}

para usar el Iterator
Iterator<Map.Entry> it = ColeccionMapa.getIterator();
while(it.hasNext())
{
  map.Entry entry = it.next;
  Obj obj = (Obj) entry.getValue();
}

----------------------------------------------------
GRABAR
public void grabar(JSONObject object, String archivo)
{
  Filewriter file = new Filewriter(archivo + ".json");
  file.write(object.toString());
  flush
  close
}

JsonObject.put("clave", objeto);
grabar(jsonArray, archivo);
----------------------------------------------------
LEER
public String leer(String archivo)
{
  String cont="";
  cont = new String(Files.ReadAllBytes(Paths.get(archivo + ".json")));
  return cont;
}

String jsonObjectArray = leer (archivo);
JSONObject1 = JSONArray.getJSONObject(i);
JSONObject2 = JSONObject1.getString("nombre");
