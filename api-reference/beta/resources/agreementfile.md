---
title: agreementFile リソースの種類
description: テナントが azure Active Directory (azure AD) を使用して管理する、カスタマイズ可能な使用許諾契約書ファイルを表します。 このファイルには、アグリーメントファイルのメタデータが含まれます (たとえば、名前、言語、および既定のファイルであるかどうか)。
localization_priority: Normal
ms.openlocfilehash: b914feecfc91d71c525711f725bf4a533d44a6b1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328619"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="556be-104">agreementFile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="556be-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="556be-105">テナントが azure Active Directory (azure AD) を使用して管理する、カスタマイズ可能な使用許諾契約書ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="556be-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="556be-106">このファイルには、アグリーメントファイルのメタデータが含まれます (たとえば、名前、言語、および既定のファイルであるかどうか)。</span><span class="sxs-lookup"><span data-stu-id="556be-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="556be-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="556be-107">Properties</span></span>
| <span data-ttu-id="556be-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="556be-108">Property</span></span>     | <span data-ttu-id="556be-109">型</span><span class="sxs-lookup"><span data-stu-id="556be-109">Type</span></span>        | <span data-ttu-id="556be-110">説明</span><span class="sxs-lookup"><span data-stu-id="556be-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="556be-111">fileData</span><span class="sxs-lookup"><span data-stu-id="556be-111">fileData</span></span>|[<span data-ttu-id="556be-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="556be-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="556be-113">使用条件を表すデータ。 PDF ドキュメント。</span><span class="sxs-lookup"><span data-stu-id="556be-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="556be-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="556be-114">Read-only.</span></span>|
|<span data-ttu-id="556be-115">fileName</span><span class="sxs-lookup"><span data-stu-id="556be-115">fileName</span></span>|<span data-ttu-id="556be-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="556be-116">String</span></span>|<span data-ttu-id="556be-117">アグリーメントファイルの名前 (たとえば、「お持ちの形式」)。</span><span class="sxs-lookup"><span data-stu-id="556be-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="556be-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="556be-118">Read-only.</span></span>|
|<span data-ttu-id="556be-119">id</span><span class="sxs-lookup"><span data-stu-id="556be-119">id</span></span>|<span data-ttu-id="556be-120">String</span><span class="sxs-lookup"><span data-stu-id="556be-120">String</span></span>|<span data-ttu-id="556be-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="556be-121">Read-only.</span></span>|
|<span data-ttu-id="556be-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="556be-122">isDefault</span></span>|<span data-ttu-id="556be-123">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="556be-123">Boolean</span></span>|<span data-ttu-id="556be-124">クライアントの優先度に一致するカルチャがない場合に、これが既定のアグリーメントファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="556be-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="556be-125">ファイルが既定として設定されていない場合は、最初のファイルが既定として扱われます。</span><span class="sxs-lookup"><span data-stu-id="556be-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="556be-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="556be-126">Read-only.</span></span>|
|<span data-ttu-id="556be-127">language</span><span class="sxs-lookup"><span data-stu-id="556be-127">language</span></span>|<span data-ttu-id="556be-128">String</span><span class="sxs-lookup"><span data-stu-id="556be-128">String</span></span>|<span data-ttu-id="556be-129">languagecode2-country/regioncode2 という形式の、アグリーメントファイルのカルチャ。</span><span class="sxs-lookup"><span data-stu-id="556be-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="556be-130">languagecode2 は、ISO 639-1 から派生した、小文字の2文字のコードです。</span><span class="sxs-lookup"><span data-stu-id="556be-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="556be-131">country/regioncode2 は ISO 3166 から派生し、通常は2つの大文字または BCP-47 language タグ (例: en-us) で構成されます。</span><span class="sxs-lookup"><span data-stu-id="556be-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="556be-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="556be-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="556be-133">関係</span><span class="sxs-lookup"><span data-stu-id="556be-133">Relationships</span></span>
<span data-ttu-id="556be-134">なし。</span><span class="sxs-lookup"><span data-stu-id="556be-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="556be-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="556be-135">JSON representation</span></span>

<span data-ttu-id="556be-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="556be-136">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
