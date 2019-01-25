---
title: programControlType リソースの種類
description: 'Azure AD にアクセスが機能を確認、アクセス確認の種類を示すために、プログラムにコントロールをコントロールに関連付けることが、ときにプログラムのコントロールの種類を使用します。  '
localization_priority: Normal
ms.openlocfilehash: 8b17a0f30fbdceb6b6da24d5cbe972223acb29b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519704"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="5138c-103">programControlType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5138c-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5138c-104">機能では、Azure AD[アクセスの確認](accessreviews-root.md)は、プログラムのコントロールの種類はコントロールは、アクセス確認の種類を示すためにも、プログラムにコントロールを関連付ける場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="5138c-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="5138c-105">プログラムのコントロール型オブジェクトは、グローバル管理者 onboards アクセスを使用するテナント機能を確認するときに自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="5138c-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="5138c-106">コントロールの種類を追加したプログラムは作成されません。</span><span class="sxs-lookup"><span data-stu-id="5138c-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="5138c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5138c-107">Methods</span></span>

| <span data-ttu-id="5138c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5138c-108">Method</span></span>           | <span data-ttu-id="5138c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5138c-109">Return Type</span></span>    |<span data-ttu-id="5138c-110">説明</span><span class="sxs-lookup"><span data-stu-id="5138c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5138c-111">リスト programControlTypes</span><span class="sxs-lookup"><span data-stu-id="5138c-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="5138c-112">[programControlType](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5138c-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="5138c-113">プログラムのコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5138c-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="5138c-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5138c-114">Properties</span></span>
| <span data-ttu-id="5138c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5138c-115">Property</span></span>     | <span data-ttu-id="5138c-116">型</span><span class="sxs-lookup"><span data-stu-id="5138c-116">Type</span></span>   |<span data-ttu-id="5138c-117">説明</span><span class="sxs-lookup"><span data-stu-id="5138c-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="5138c-118">プログラムのコントロールの種類の機能に割り当てられた識別子</span><span class="sxs-lookup"><span data-stu-id="5138c-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="5138c-119">プログラムのコントロールの種類の名前</span><span class="sxs-lookup"><span data-stu-id="5138c-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="5138c-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5138c-120">Relationships</span></span>

<span data-ttu-id="5138c-121">なし。</span><span class="sxs-lookup"><span data-stu-id="5138c-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="5138c-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="5138c-122">See also</span></span>

| <span data-ttu-id="5138c-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="5138c-123">Method</span></span>           | <span data-ttu-id="5138c-124">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5138c-124">Return Type</span></span>    |<span data-ttu-id="5138c-125">説明</span><span class="sxs-lookup"><span data-stu-id="5138c-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5138c-126">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="5138c-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="5138c-127">デバッギング</span><span class="sxs-lookup"><span data-stu-id="5138c-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="5138c-128">デバッギングをプログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="5138c-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5138c-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5138c-129">JSON representation</span></span>

<span data-ttu-id="5138c-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5138c-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontroltype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
