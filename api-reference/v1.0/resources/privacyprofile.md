# <a name="privacyprofile-resource-type"></a><span data-ttu-id="02bd8-101">privacyProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02bd8-101">privacyProfile resource type</span></span>

<span data-ttu-id="02bd8-102">会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="02bd8-102">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="02bd8-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02bd8-103">Properties</span></span>
| <span data-ttu-id="02bd8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02bd8-104">Property</span></span>   | <span data-ttu-id="02bd8-105">型</span><span class="sxs-lookup"><span data-stu-id="02bd8-105">Type</span></span>|<span data-ttu-id="02bd8-106">説明</span><span class="sxs-lookup"><span data-stu-id="02bd8-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02bd8-107">contactEmail</span><span class="sxs-lookup"><span data-stu-id="02bd8-107">contactEmail</span></span>|<span data-ttu-id="02bd8-108">String</span><span class="sxs-lookup"><span data-stu-id="02bd8-108">String</span></span>| <span data-ttu-id="02bd8-109">プライバシー ステートメントの連絡先担当者の有効な SMTP メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="02bd8-109">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="02bd8-110">省略可。</span><span class="sxs-lookup"><span data-stu-id="02bd8-110">Not required</span></span>|
|<span data-ttu-id="02bd8-111">statementUrl</span><span class="sxs-lookup"><span data-stu-id="02bd8-111">statementUrl</span></span>|<span data-ttu-id="02bd8-112">String</span><span class="sxs-lookup"><span data-stu-id="02bd8-112">String</span></span>| <span data-ttu-id="02bd8-113">http:// または https:// で始まる有効な URL 形式。</span><span class="sxs-lookup"><span data-stu-id="02bd8-113">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="02bd8-114">最大の長さは 255 文字です。</span><span class="sxs-lookup"><span data-stu-id="02bd8-114">The maximum length is 255 characters.</span></span> <span data-ttu-id="02bd8-115">会社のプライバシー ステートメントに誘導する URL。</span><span class="sxs-lookup"><span data-stu-id="02bd8-115">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="02bd8-116">省略可。</span><span class="sxs-lookup"><span data-stu-id="02bd8-116">Not required</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02bd8-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02bd8-117">JSON representation</span></span>

<span data-ttu-id="02bd8-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="02bd8-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```