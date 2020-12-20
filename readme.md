# Rethink Autocomplete

https://drive.google.com/file/d/1t-h0blhJePqqwrOg7O5L3AV84yFnSRBv/view?usp=sharing

Due to time constraint, I've [react-search-ui]"https://www.npmjs.com/package/@elastic/react-search-ui", a powerful search engine powered by lucene, with an intuitive front-end. react-search-ui has a lot of additional features such as fitering and sorting. To keep the code size small, I've stripped away a lot of the additional features.

In my initial write-ups i suggested using MySQL for storing the NGram similarity. After some study I realized that it is not very effective in storing big matrix. Using an infrastructure such as Hadoop with HBase might be a better choice.

# Assumptions

(altered according to time constraint)

- Start to suggest uppon entering one character

# Scope

Must have:

- Suggestion on each character - done
- Search in both titles and description text

Nice to have:

- analytics on search pattern

Not in scope:

- add or update database

# run locally

- FORK this repo
- `cd backend`
- `npm install & npm run dev`
- open `localhost:3000`
- enjoy

# TODO

(in addition to scope)

- benchmark different indexing stragies: Edge-Ngram vs Prefix Query vs Completion Suggester.
