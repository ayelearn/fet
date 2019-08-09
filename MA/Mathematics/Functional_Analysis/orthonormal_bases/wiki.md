The following text has been accessed from https://en.wikipedia.org/wiki/Orthonormal_basis at Fri Aug 9 02:38:37 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Orthonormal basis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, particularly linear_algebra, an orthonormal basis for an inner
product_space V with finite dimension is a basis for V whose vectors are
orthonormal, that is, they are all unit_vectors and orthogonal to each other.
[1][2][3] For example, the standard_basis for a Euclidean_space Rn is an
orthonormal basis, where the relevant inner product is the dot_product of
vectors. The image of the standard basis under a rotation or reflection (or any
orthogonal_transformation) is also orthonormal, and every orthonormal basis for
Rn arises in this fashion.
For a general inner product space V, an orthonormal basis can be used to define
normalized orthogonal_coordinates on V. Under these coordinates, the inner
product becomes a dot product of vectors. Thus the presence of an orthonormal
basis reduces the study of a finite-dimensional inner product space to the
study of Rn under dot product. Every finite-dimensional inner product space has
an orthonormal basis, which may be obtained from an arbitrary basis using the
GramâSchmidt_process.
In functional_analysis, the concept of an orthonormal basis can be generalized
to arbitrary (infinite-dimensional) inner_product_spaces.[4] Given a pre-
Hilbert space H, an orthonormal basis for H is an orthonormal set of vectors
with the property that every vector in H can be written as an infinite_linear
combination of the vectors in the basis. In this case, the orthonormal basis is
sometimes called a Hilbert basis for H. Note that an orthonormal basis in this
sense is not generally a Hamel_basis, since infinite linear combinations are
required. Specifically, the linear_span of the basis must be dense in H, but it
may not be the entire space.
If we go on to Hilbert_spaces, a non-orthonormal set of vectors having the same
linear span as an orthonormal basis may not be a basis at all. For instance,
any square-integrable_function on the interval [â1, 1] can be expressed
(almost_everywhere) as an infinite sum of Legendre_polynomials (an orthonomal
basis), but not necessarily as an infinite sum of the monomials xn.
⁰
***** Contents *****
    * 1_Examples
    * 2_Basic_formula
    * 3_Incomplete_orthogonal_sets
    * 4_Existence
    * 5_As_a_homogeneous_space
    * 6_See_also
    * 7_References
***** Examples[edit] *****
    * The set of vectors {e1 = (1, 0, 0), e2 = (0, 1, 0), e3 = (0, 0, 1)} (the
      standard basis) forms an orthonormal basis of R3.
            Proof: A straightforward computation shows that the inner products
            of these vectors equals zero, &#x27e8;e1, e2&#x27e9; = &#x27e8;e1,
            e3&#x27e9; = &#x27e8;e2, e3&#x27e9; = 0 and that each of their
            magnitudes equals one, ||e1|| = ||e2|| = ||e3|| = 1. This means
            that {e1, e2, e3}  is an orthonormal set. All vectors (x, y, z) in
            R3 can be expressed as a sum of the basis vectors scaled
                     ( x , y , z ) = x  e  1   + y  e  2   + z  e  3   ,
                  {\displaystyle (x,y,z)=xe_{1}+ye_{2}+ze_{3},\,}  [(x,y,z)=xe_
                  {1}+ye_{2}+ze_{3},\,]
            so {e1, e2, e3}  spans R3 and hence must be a basis. It may also be
            shown that the standard basis rotated about an axis through the
            origin or reflected in a plane through the origin forms an
            orthonormal basis of R3.
    * Notice that an orthogonal_transformation of the standard inner-product
      space     (   R   n   , &#x27E8; &#x22C5; , &#x22C5; &#x27E9; )
      {\displaystyle (\mathbb {R} ^{n},\langle \cdot ,\cdot \rangle )}  [
      {\displaystyle (\mathbb {R} ^{n},\langle \cdot ,\cdot \rangle )}] can be
      used to construct other orthogonal bases of       R   n
      {\displaystyle \mathbb {R} ^{n}}  [\mathbb {R} ^{n}].
    * The set {fn : n â Z}  with fn(x) = exp(2Ïinx) forms an orthonormal
      basis of the space of functions with finite Lebesgue integrals, L2(
      [0,1]), with respect to the 2-norm. This is fundamental to the study of
      Fourier_series.
    * The set {eb : b â B}  with eb(c) = 1 if b = c and 0 otherwise forms an
      orthonormal basis of â2(B).
    * Eigenfunctions of a SturmâLiouville_eigenproblem.
    * An orthogonal_matrix is a matrix whose column vectors form an orthonormal
      set.
***** Basic formula[edit] *****
If B is an orthogonal basis of H, then every element x of H may be written as
         x =  &#x2211;  b &#x2208; B      &#x27E8; x , b &#x27E9;   &#x2016; b
      &#x2016;  2      b .   {\displaystyle x=\sum _{b\in B}{\langle x,b\rangle
      \over \lVert b\rVert ^{2}}b.}  [x=\sum _{b\in B}{\langle x,b\rangle
      \over \lVert b\rVert ^{2}}b.]
When B is orthonormal, this simplifies to
         x =  &#x2211;  b &#x2208; B   &#x27E8; x , b &#x27E9; b
      {\displaystyle x=\sum _{b\in B}\langle x,b\rangle b}  [x=\sum _{b\in
      B}\langle x,b\rangle b]
and the square of the norm of x can be given by
         &#x2016; x  &#x2016;  2   =  &#x2211;  b &#x2208; B    |  &#x27E8; x ,
      b &#x27E9;   |   2   .   {\displaystyle \|x\|^{2}=\sum _{b\in B}|\langle
      x,b\rangle |^{2}.}  [\|x\|^{2}=\sum _{b\in B}|\langle x,b\rangle |^{2}.]
Even if B is uncountable, only countably many terms in this sum will be non-
zero, and the expression is therefore well-defined. This sum is also called the
Fourier_expansion of x, and the formula is usually known as Parseval's
identity.
If B is an orthonormal basis of H, then H is isomorphic to â 2(B) in the
following sense: there exists a bijective linear map Î¦ : H â â2(B) such
that
         &#x27E8; &#x03A6; ( x ) , &#x03A6; ( y ) &#x27E9; = &#x27E8; x , y
      &#x27E9;   {\displaystyle \langle \Phi (x),\Phi (y)\rangle =\langle
      x,y\rangle }  [\langle \Phi (x),\Phi (y)\rangle =\langle x,y\rangle ]
for all x and y in H.
***** Incomplete orthogonal sets[edit] *****
Given a Hilbert space H and a set S of mutually orthogonal vectors in H, we can
take the smallest closed linear subspace V of H containing S. Then S will be an
orthogonal basis of V; which may of course be smaller than H itself, being an
incomplete orthogonal set, or be H, when it is a complete orthogonal set.
***** Existence[edit] *****
Using Zorn's_lemma and the GramâSchmidt_process (or more simply well-ordering
and transfinite recursion), one can show that every Hilbert space admits a
basis, but not orthonormal base[5]; furthermore, any two orthonormal bases of
the same space have the same cardinality (this can be proven in a manner akin
to that of the proof of the usual dimension_theorem_for_vector_spaces, with
separate cases depending on whether the larger basis candidate is countable or
not). A Hilbert space is separable if and only if it admits a countable
orthonormal basis. (One can prove this last statement without using the axiom
of choice).
***** As a homogeneous space[edit] *****
Main article: Stiefel_manifold
The set of orthonormal bases for a space is a principal_homogeneous_space for
the orthogonal_group O(n), and is called the Stiefel_manifold      V  n   (   R
n   )   {\displaystyle V_{n}(\mathbf {R} ^{n})}  [V_{n}(\mathbf {R} ^{n})] of
orthonormal n-frames.
In other words, the space of orthonormal bases is like the orthogonal group,
but without a choice of base point: given an orthogonal space, there is no
natural choice of orthonormal basis, but once one is given one, there is a one-
to-one correspondence between bases and the orthogonal group. Concretely, a
linear map is determined by where it sends a given basis: just as an invertible
map can take any basis to any other basis, an orthogonal map can take any
orthogonal basis to any other orthogonal basis.
The other Stiefel manifolds      V  k   (   R   n   )   {\displaystyle V_{k}
(\mathbf {R} ^{n})}  [V_{k}(\mathbf {R} ^{n})] for     k < n   {\displaystyle
k<n}  [k<n] of incomplete orthonormal bases (orthonormal k-frames) are still
homogeneous spaces for the orthogonal group, but not principal homogeneous
spaces: any k-frame can be taken to any other k-frame by an orthogonal map, but
this map is not uniquely determined.
***** See also[edit] *****
    * Basis_(linear_algebra)
    * Orthonormal_frame
    * Schauder_basis
    * Total_set
***** References[edit] *****
   1. ^Lay, David C. (2006). Linear Algebra and Its Applications (3rd ed.).
      AddisonâWesley. ISBN 0-321-28713-4.
   2. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
      .citation q{quotes:"\"""\"""'""'"}.mw-parser-output .citation .cs1-lock-
      free a{background:url("//upload.wikimedia.org/wikipedia/commons/thumb/6/
      65/Lock-green.svg/9px-Lock-green.svg.png")no-repeat;background-position:
      right .1em center}.mw-parser-output .citation .cs1-lock-limited a,.mw-
      parser-output .citation .cs1-lock-registration a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/d/d6/Lock-gray-alt-2.svg/
      9px-Lock-gray-alt-2.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output .citation .cs1-lock-subscription a{background:
      url("//upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Lock-red-alt-
      2.svg/9px-Lock-red-alt-2.svg.png")no-repeat;background-position:right
      .1em center}.mw-parser-output .cs1-subscription,.mw-parser-output .cs1-
      registration{color:#555}.mw-parser-output .cs1-subscription span,.mw-
      parser-output .cs1-registration span{border-bottom:1px dotted;cursor:
      help}.mw-parser-output .cs1-ws-icon a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Wikisource-logo.svg/
      12px-Wikisource-logo.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output code.cs1-code{color:inherit;background:
      inherit;border:inherit;padding:inherit}.mw-parser-output .cs1-hidden-
      error{display:none;font-size:100%}.mw-parser-output .cs1-visible-error
      {font-size:100%}.mw-parser-output .cs1-maint{display:none;color:
      #33aa33;margin-left:0.3em}.mw-parser-output .cs1-subscription,.mw-parser-
      output .cs1-registration,.mw-parser-output .cs1-format{font-size:95%}.mw-
      parser-output .cs1-kern-left,.mw-parser-output .cs1-kern-wl-left{padding-
      left:0.2em}.mw-parser-output .cs1-kern-right,.mw-parser-output .cs1-kern-
      wl-right{padding-right:0.2em}
   3. ^Strang,_Gilbert (2006). Linear Algebra and Its Applications (4th ed.).
      Brooks_Cole. ISBN 0-03-010567-6.
   4. ^Axler, Sheldon (2002). Linear Algebra Done Right (2nd ed.). Springer.
      ISBN 0-387-98258-2.
   5. ^Rudin,_Walter (1987). Real & Complex Analysis. McGraw-Hill. ISBN 0-07-
      054234-1.
   6. ^  Linear Functional Analysis Authors: Rynne, Bryan, Youngson, M.A. page
      79

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Orthonormal_basis&oldid=903741736"
Categories:
    * Linear_algebra
    * Functional_analysis
    * Fourier_analysis
***** Navigation menu *****
**** Personal tools ****
    * Not logged in
    * Talk
    * Contributions
    * Create_account
    * Log_in
**** Namespaces ****
    * Article
    * Talk
⁰
**** Variants ****
**** Views ****
    * Read
    * Edit
    * View_history
⁰
**** More ****
**** Search ****
[Unknown INPUT type][Search][Go]
**** Navigation ****
    * Main_page
    * Contents
    * Featured_content
    * Current_events
    * Random_article
    * Donate_to_Wikipedia
    * Wikipedia_store
**** Interaction ****
    * Help
    * About_Wikipedia
    * Community_portal
    * Recent_changes
    * Contact_page
**** Tools ****
    * What_links_here
    * Related_changes
    * Upload_file
    * Special_pages
    * Permanent_link
    * Page_information
    * Wikidata_item
    * Cite_this_page
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 27 June 2019, at 17:32 (UTC).
    * Text is available under the Creative_Commons_Attribution-ShareAlike
      License; additional terms may apply. By using this site, you agree to the
      Terms_of_Use and Privacy_Policy. WikipediaÂ® is a registered trademark of
      the Wikimedia_Foundation,_Inc., a non-profit organization.
    * Privacy_policy
    * About_Wikipedia
    * Disclaimers
    * Contact_Wikipedia
    * Developers
    * Cookie_statement
    * Mobile_view
    * [Wikimedia_Foundation]
    * [Powered_by_MediaWiki]
