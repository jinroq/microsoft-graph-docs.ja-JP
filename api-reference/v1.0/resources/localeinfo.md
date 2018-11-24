# <a name="localeinfo-resource-type"></a><span data-ttu-id="76333-101">localeInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76333-101">localeInfo resource type</span></span>

<span data-ttu-id="76333-102">サインインしているユーザーの優先言語および国/地域を含むロケールに関する情報。</span><span class="sxs-lookup"><span data-stu-id="76333-102">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="76333-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76333-103">Properties</span></span>
| <span data-ttu-id="76333-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76333-104">Property</span></span>     | <span data-ttu-id="76333-105">型</span><span class="sxs-lookup"><span data-stu-id="76333-105">Type</span></span>   |<span data-ttu-id="76333-106">説明</span><span class="sxs-lookup"><span data-stu-id="76333-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76333-107">locale</span><span class="sxs-lookup"><span data-stu-id="76333-107">locale</span></span>|<span data-ttu-id="76333-108">文字列</span><span class="sxs-lookup"><span data-stu-id="76333-108">string</span></span>|<span data-ttu-id="76333-p101">ユーザーのロケールを表します。ユーザーの優先言語および国/地域が含まれます。たとえば、"en-us"。言語のコンポーネントは [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) で定義されている 2 文字のコードに従い、国のコンポーネントは [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm) で定義されている 2 文字のコードに従います。</span><span class="sxs-lookup"><span data-stu-id="76333-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="76333-112">displayName</span><span class="sxs-lookup"><span data-stu-id="76333-112">displayName</span></span>|<span data-ttu-id="76333-113">string</span><span class="sxs-lookup"><span data-stu-id="76333-113">string</span></span>|<span data-ttu-id="76333-114">たとえば "English (United States)" のように、ユーザーのロケールを自然言語で表す名前。</span><span class="sxs-lookup"><span data-stu-id="76333-114">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76333-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76333-115">JSON representation</span></span>

<span data-ttu-id="76333-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76333-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->