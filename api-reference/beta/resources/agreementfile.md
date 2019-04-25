---
title: agreementFile リソースの種類
description: テナントが azure Active Directory (azure AD) を使用して管理する、カスタマイズ可能な使用許諾契約書ファイルを表します。 このファイルには、アグリーメントファイルのメタデータが含まれます (たとえば、名前、言語、および既定のファイルであるかどうか)。
localization_priority: Normal
ms.openlocfilehash: 446173e83d32af96f938cbee15964ea204a62f7e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535754"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="7328d-104">agreementFile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7328d-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7328d-105">テナントが azure Active Directory (azure AD) を使用して管理する、カスタマイズ可能な使用許諾契約書ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="7328d-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="7328d-106">このファイルには、アグリーメントファイルのメタデータが含まれます (たとえば、名前、言語、および既定のファイルであるかどうか)。</span><span class="sxs-lookup"><span data-stu-id="7328d-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="7328d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7328d-107">Properties</span></span>
| <span data-ttu-id="7328d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7328d-108">Property</span></span>     | <span data-ttu-id="7328d-109">型</span><span class="sxs-lookup"><span data-stu-id="7328d-109">Type</span></span>        | <span data-ttu-id="7328d-110">説明</span><span class="sxs-lookup"><span data-stu-id="7328d-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7328d-111">fileData</span><span class="sxs-lookup"><span data-stu-id="7328d-111">fileData</span></span>|[<span data-ttu-id="7328d-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="7328d-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="7328d-113">使用条件を表すデータ。 PDF ドキュメント。</span><span class="sxs-lookup"><span data-stu-id="7328d-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="7328d-114">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="7328d-114">Read-only.</span></span>|
|<span data-ttu-id="7328d-115">fileName</span><span class="sxs-lookup"><span data-stu-id="7328d-115">fileName</span></span>|<span data-ttu-id="7328d-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7328d-116">String</span></span>|<span data-ttu-id="7328d-117">アグリーメントファイルの名前 (たとえば、「お持ちの形式」)。</span><span class="sxs-lookup"><span data-stu-id="7328d-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="7328d-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7328d-118">Read-only.</span></span>|
|<span data-ttu-id="7328d-119">id</span><span class="sxs-lookup"><span data-stu-id="7328d-119">id</span></span>|<span data-ttu-id="7328d-120">String</span><span class="sxs-lookup"><span data-stu-id="7328d-120">String</span></span>|<span data-ttu-id="7328d-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7328d-121">Read-only.</span></span>|
|<span data-ttu-id="7328d-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="7328d-122">isDefault</span></span>|<span data-ttu-id="7328d-123">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="7328d-123">Boolean</span></span>|<span data-ttu-id="7328d-124">クライアントの優先度に一致するカルチャがない場合に、これが既定のアグリーメントファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7328d-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="7328d-125">ファイルが既定として設定されていない場合は、最初のファイルが既定として扱われます。</span><span class="sxs-lookup"><span data-stu-id="7328d-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="7328d-126">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="7328d-126">Read-only.</span></span>|
|<span data-ttu-id="7328d-127">language</span><span class="sxs-lookup"><span data-stu-id="7328d-127">language</span></span>|<span data-ttu-id="7328d-128">String</span><span class="sxs-lookup"><span data-stu-id="7328d-128">String</span></span>|<span data-ttu-id="7328d-129">languagecode2-country/regioncode2 という形式の、アグリーメントファイルのカルチャ。</span><span class="sxs-lookup"><span data-stu-id="7328d-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="7328d-130">languagecode2 は、ISO 639-1 から派生した、小文字の2文字のコードです。</span><span class="sxs-lookup"><span data-stu-id="7328d-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="7328d-131">country/regioncode2 は ISO 3166 から派生し、通常は2つの大文字または BCP-47 language タグ (例: en-us) で構成されます。</span><span class="sxs-lookup"><span data-stu-id="7328d-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="7328d-132">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="7328d-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7328d-133">関係</span><span class="sxs-lookup"><span data-stu-id="7328d-133">Relationships</span></span>
<span data-ttu-id="7328d-134">なし。</span><span class="sxs-lookup"><span data-stu-id="7328d-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7328d-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7328d-135">JSON representation</span></span>

<span data-ttu-id="7328d-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7328d-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
