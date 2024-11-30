     const  tabbtn = [
      {name : "1tab"},
      {name : "2tab"},
      {name : "3tab"}
     ]
          const [tab, setTab] = useState(tabbtn.name);

 
 <div className="bg-white absolute bottom-0 left-0">
            {tabbtn.map((items, index) => (
              <button
                key={index}
                onClick={() => setTab(items.name)}
                className="w-[100px] h-[100px] bg-[black] text-white "
              >
                {items.name}
              </button>
            ))}

            <div className="w-[500px] h-[500px] bg-black text-white">
              {tab === "1tab"
                ? "1tab"
                : tab === "2tab"
                ? "2tab"
                : tab === "3tab" && "3tab"}
            </div>
          </div>




