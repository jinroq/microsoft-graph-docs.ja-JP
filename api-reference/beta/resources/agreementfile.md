---
title: agreementFile リソースの種類
description: Azure Active Directory (AD の Azure) とテナントを管理する使用許諾契約書ファイルのカスタマイズ可能な条件を表します。 契約書のファイルについてのメタデータが含まれています (たとえば、名前、言語、既定のファイルであるかどうかと)。
localization_priority: Normal
ms.openlocfilehash: 446173e83d32af96f938cbee15964ea204a62f7e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511430"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="d098f-104">agreementFile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d098f-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d098f-105">Azure Active Directory (AD の Azure) とテナントを管理する使用許諾契約書ファイルのカスタマイズ可能な条件を表します。</span><span class="sxs-lookup"><span data-stu-id="d098f-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="d098f-106">契約書のファイルについてのメタデータが含まれています (たとえば、名前、言語、既定のファイルであるかどうかと)。</span><span class="sxs-lookup"><span data-stu-id="d098f-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="d098f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d098f-107">Properties</span></span>
| <span data-ttu-id="d098f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d098f-108">Property</span></span>     | <span data-ttu-id="d098f-109">型</span><span class="sxs-lookup"><span data-stu-id="d098f-109">Type</span></span>        | <span data-ttu-id="d098f-110">説明</span><span class="sxs-lookup"><span data-stu-id="d098f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d098f-111">fileData</span><span class="sxs-lookup"><span data-stu-id="d098f-111">fileData</span></span>|[<span data-ttu-id="d098f-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="d098f-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="d098f-113">PDF 文書の使用の条件を表すデータです。</span><span class="sxs-lookup"><span data-stu-id="d098f-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="d098f-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d098f-114">Read-only.</span></span>|
|<span data-ttu-id="d098f-115">fileName</span><span class="sxs-lookup"><span data-stu-id="d098f-115">fileName</span></span>|<span data-ttu-id="d098f-116">String</span><span class="sxs-lookup"><span data-stu-id="d098f-116">String</span></span>|<span data-ttu-id="d098f-117">契約ファイル (TOU.pdf など) の名前です。</span><span class="sxs-lookup"><span data-stu-id="d098f-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="d098f-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d098f-118">Read-only.</span></span>|
|<span data-ttu-id="d098f-119">id</span><span class="sxs-lookup"><span data-stu-id="d098f-119">id</span></span>|<span data-ttu-id="d098f-120">文字列</span><span class="sxs-lookup"><span data-stu-id="d098f-120">String</span></span>|<span data-ttu-id="d098f-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d098f-121">Read-only.</span></span>|
|<span data-ttu-id="d098f-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="d098f-122">isDefault</span></span>|<span data-ttu-id="d098f-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="d098f-123">Boolean</span></span>|<span data-ttu-id="d098f-124">クライアント基本設定と一致する、カルチャの場合、既定の契約書ファイルはかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d098f-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="d098f-125">ファイルの [なし] は既定値としてマークすると、1 つ目は既定値として扱われます。</span><span class="sxs-lookup"><span data-stu-id="d098f-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="d098f-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d098f-126">Read-only.</span></span>|
|<span data-ttu-id="d098f-127">language</span><span class="sxs-lookup"><span data-stu-id="d098f-127">language</span></span>|<span data-ttu-id="d098f-128">String</span><span class="sxs-lookup"><span data-stu-id="d098f-128">String</span></span>|<span data-ttu-id="d098f-129">形式 languagecode2 の国と regioncode2 の契約書ファイルのカルチャです。</span><span class="sxs-lookup"><span data-stu-id="d098f-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="d098f-130">languagecode2 は、小文字の ISO 639-1 から派生した 2 文字コードです。</span><span class="sxs-lookup"><span data-stu-id="d098f-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="d098f-131">国/regioncode2 では、ISO 3166 から派生し、通常は、2 つの大文字、または BCP 47 言語タグ (たとえば、EN-US)。</span><span class="sxs-lookup"><span data-stu-id="d098f-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="d098f-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d098f-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d098f-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d098f-133">Relationships</span></span>
<span data-ttu-id="d098f-134">なし。</span><span class="sxs-lookup"><span data-stu-id="d098f-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d098f-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d098f-135">JSON representation</span></span>

<span data-ttu-id="d098f-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d098f-136">The following is a JSON representation of the resource.</span></span>

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
