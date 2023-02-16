 if (fs.existsSync('../submission/README.md')) {
        const README = fs.readFileSync('../submission/README.md', 'utf8')
        expect(README).toMatch(/fullstack-decal-sp23\.github\.io\/hw2-/)
    } else {
        throw new Error('No README.md found')
    } 