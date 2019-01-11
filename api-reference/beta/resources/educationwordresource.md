---
title: educationWordResource リソースの種類
description: 'EducationResource のサブクラスです。 これは、Word ドキュメント リソースです。 関連付けられている**fileResource**ディレクトリに Word ファイルをアップロードする必要があります、 '
localization_priority: Normal
ms.openlocfilehash: 0fa366a6fb6de70d10a010cf5e0e11ffd26a3b94
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805139"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="6ba28-105">educationWordResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ba28-105">educationWordResource resource type</span></span>

> <span data-ttu-id="6ba28-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6ba28-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ba28-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ba28-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ba28-108">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="6ba28-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="6ba28-109">これは、Word ドキュメント リソースです。</span><span class="sxs-lookup"><span data-stu-id="6ba28-109">This is a Word document resource.</span></span> <span data-ttu-id="6ba28-110">Word ファイルを送信または割り当てに関連付けられている**fileResource**ディレクトリにアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ba28-110">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="6ba28-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ba28-111">Properties</span></span>
| <span data-ttu-id="6ba28-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ba28-112">Property</span></span>     | <span data-ttu-id="6ba28-113">種類</span><span class="sxs-lookup"><span data-stu-id="6ba28-113">Type</span></span>   |<span data-ttu-id="6ba28-114">説明</span><span class="sxs-lookup"><span data-stu-id="6ba28-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ba28-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="6ba28-115">fileUrl</span></span>|<span data-ttu-id="6ba28-116">String</span><span class="sxs-lookup"><span data-stu-id="6ba28-116">String</span></span>|<span data-ttu-id="6ba28-117">ディスク上のファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="6ba28-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ba28-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ba28-118">JSON representation</span></span>

<span data-ttu-id="6ba28-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6ba28-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
