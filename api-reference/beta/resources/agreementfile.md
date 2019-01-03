---
title: agreementFile リソースの種類
description: Azure Active Directory (AD の Azure) とテナントを管理する使用許諾契約書ファイルのカスタマイズ可能な条件を表します。 契約書のファイルについてのメタデータが含まれています (たとえば、名前、言語、既定のファイルであるかどうかと)。
ms.openlocfilehash: f099715fd25fbae9d7b2a94d6de841b8766c30e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070279"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="e32e2-104">agreementFile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e32e2-104">agreementFile resource type</span></span>

> <span data-ttu-id="e32e2-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e32e2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e32e2-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e32e2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e32e2-107">Azure Active Directory (AD の Azure) とテナントを管理する使用許諾契約書ファイルのカスタマイズ可能な条件を表します。</span><span class="sxs-lookup"><span data-stu-id="e32e2-107">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="e32e2-108">契約書のファイルについてのメタデータが含まれています (たとえば、名前、言語、既定のファイルであるかどうかと)。</span><span class="sxs-lookup"><span data-stu-id="e32e2-108">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="e32e2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e32e2-109">Properties</span></span>
| <span data-ttu-id="e32e2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e32e2-110">Property</span></span>     | <span data-ttu-id="e32e2-111">型</span><span class="sxs-lookup"><span data-stu-id="e32e2-111">Type</span></span>        | <span data-ttu-id="e32e2-112">説明</span><span class="sxs-lookup"><span data-stu-id="e32e2-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e32e2-113">fileData</span><span class="sxs-lookup"><span data-stu-id="e32e2-113">fileData</span></span>|[<span data-ttu-id="e32e2-114">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="e32e2-114">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="e32e2-115">PDF 文書の使用の条件を表すデータです。</span><span class="sxs-lookup"><span data-stu-id="e32e2-115">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="e32e2-116">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e32e2-116">Read-only.</span></span>|
|<span data-ttu-id="e32e2-117">fileName</span><span class="sxs-lookup"><span data-stu-id="e32e2-117">fileName</span></span>|<span data-ttu-id="e32e2-118">String</span><span class="sxs-lookup"><span data-stu-id="e32e2-118">String</span></span>|<span data-ttu-id="e32e2-119">契約ファイル (TOU.pdf など) の名前です。</span><span class="sxs-lookup"><span data-stu-id="e32e2-119">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="e32e2-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e32e2-120">Read-only.</span></span>|
|<span data-ttu-id="e32e2-121">id</span><span class="sxs-lookup"><span data-stu-id="e32e2-121">id</span></span>|<span data-ttu-id="e32e2-122">String</span><span class="sxs-lookup"><span data-stu-id="e32e2-122">String</span></span>|<span data-ttu-id="e32e2-123">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e32e2-123">Read-only.</span></span>|
|<span data-ttu-id="e32e2-124">isDefault</span><span class="sxs-lookup"><span data-stu-id="e32e2-124">isDefault</span></span>|<span data-ttu-id="e32e2-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="e32e2-125">Boolean</span></span>|<span data-ttu-id="e32e2-126">クライアント基本設定と一致する、カルチャの場合、既定の契約書ファイルはかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e32e2-126">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="e32e2-127">ファイルの [なし] は既定値としてマークすると、1 つ目は既定値として扱われます。</span><span class="sxs-lookup"><span data-stu-id="e32e2-127">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="e32e2-128">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e32e2-128">Read-only.</span></span>|
|<span data-ttu-id="e32e2-129">language</span><span class="sxs-lookup"><span data-stu-id="e32e2-129">language</span></span>|<span data-ttu-id="e32e2-130">String</span><span class="sxs-lookup"><span data-stu-id="e32e2-130">String</span></span>|<span data-ttu-id="e32e2-131">形式 languagecode2 の国と regioncode2 の契約書ファイルのカルチャです。</span><span class="sxs-lookup"><span data-stu-id="e32e2-131">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="e32e2-132">languagecode2 は、小文字の ISO 639-1 から派生した 2 文字コードです。</span><span class="sxs-lookup"><span data-stu-id="e32e2-132">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="e32e2-133">国/regioncode2 では、ISO 3166 から派生し、通常は、2 つの大文字、または BCP 47 言語タグ (たとえば、EN-US)。</span><span class="sxs-lookup"><span data-stu-id="e32e2-133">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="e32e2-134">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e32e2-134">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e32e2-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e32e2-135">Relationships</span></span>
<span data-ttu-id="e32e2-136">なし。</span><span class="sxs-lookup"><span data-stu-id="e32e2-136">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e32e2-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e32e2-137">JSON representation</span></span>

<span data-ttu-id="e32e2-138">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e32e2-138">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->