---
title: educationFileResource リソースの種類
description: 送信または割り当てに関連付けられているファイル オブジェクトを表す educationResource のサブクラスです。  この例では、ファイルは特別なファイル (Word、Excel、およびなど) のいずれかがファイル システム内で特別な処理がないです。 このリソースに接続されている送信または割り当てに関連付けられている**resourceFolder**では、ファイル リソースを格納してください。
ms.openlocfilehash: b3ba77b6b9243d987ad1137afe6d2206e47dadaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070551"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="7231b-105">educationFileResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7231b-105">educationFileResource resource type</span></span>

> <span data-ttu-id="7231b-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7231b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7231b-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7231b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7231b-108">送信または割り当てに関連付けられているファイル オブジェクトを表す[educationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="7231b-108">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="7231b-109">この例では、ファイルは特別なファイル (Word、Excel、およびなど) のいずれかがファイル システム内で特別な処理がないです。</span><span class="sxs-lookup"><span data-stu-id="7231b-109">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="7231b-110">このリソースに接続されている送信または割り当てに関連付けられている**resourceFolder**では、ファイル リソースを格納してください。</span><span class="sxs-lookup"><span data-stu-id="7231b-110">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="7231b-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7231b-111">Properties</span></span>
| <span data-ttu-id="7231b-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7231b-112">Property</span></span>     | <span data-ttu-id="7231b-113">型</span><span class="sxs-lookup"><span data-stu-id="7231b-113">Type</span></span>   |<span data-ttu-id="7231b-114">説明</span><span class="sxs-lookup"><span data-stu-id="7231b-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7231b-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="7231b-115">fileUrl</span></span>|<span data-ttu-id="7231b-116">String</span><span class="sxs-lookup"><span data-stu-id="7231b-116">String</span></span>|<span data-ttu-id="7231b-117">ファイル リソースのディスク上の場所です。</span><span class="sxs-lookup"><span data-stu-id="7231b-117">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7231b-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7231b-118">JSON representation</span></span>

<span data-ttu-id="7231b-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7231b-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
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
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->