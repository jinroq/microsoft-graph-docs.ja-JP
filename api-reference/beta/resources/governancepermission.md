---
title: governancePermission リソースの種類
description: '特定の governanceResource に、governanceSubject を持つアクセス許可を表します。  '
localization_priority: Normal
ms.openlocfilehash: e082ca50e5642e865b3e30859eea607df63a03b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882874"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="fa7f2-103">governancePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa7f2-103">governancePermission resource type</span></span>

> <span data-ttu-id="fa7f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fa7f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa7f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa7f2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa7f2-106">特定の[governanceResource](../resources/governanceresource.md)に、 [governanceSubject](../resources/governancesubject.md)を持つアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="fa7f2-106">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="fa7f2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa7f2-107">Properties</span></span>
| <span data-ttu-id="fa7f2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa7f2-108">Property</span></span>     | <span data-ttu-id="fa7f2-109">種類</span><span class="sxs-lookup"><span data-stu-id="fa7f2-109">Type</span></span>   |<span data-ttu-id="fa7f2-110">説明</span><span class="sxs-lookup"><span data-stu-id="fa7f2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa7f2-111">accessLevel</span><span class="sxs-lookup"><span data-stu-id="fa7f2-111">accessLevel</span></span>|<span data-ttu-id="fa7f2-112">String</span><span class="sxs-lookup"><span data-stu-id="fa7f2-112">String</span></span>|<span data-ttu-id="fa7f2-113">アクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="fa7f2-113">The access level.</span></span> <span data-ttu-id="fa7f2-114">有効な値: ``None``、 ``UserRead``、``AdminRead``と``AdminReadWrite``。</span><span class="sxs-lookup"><span data-stu-id="fa7f2-114">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="fa7f2-115">isActive</span><span class="sxs-lookup"><span data-stu-id="fa7f2-115">isActive</span></span>|<span data-ttu-id="fa7f2-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="fa7f2-116">Boolean</span></span>|<span data-ttu-id="fa7f2-117">指定する場合、リクエスターが、アクティブなロールの割り当てのアクセス レベルを持ちます。</span><span class="sxs-lookup"><span data-stu-id="fa7f2-117">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="fa7f2-118">isEligible</span><span class="sxs-lookup"><span data-stu-id="fa7f2-118">isEligible</span></span>|<span data-ttu-id="fa7f2-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="fa7f2-119">Boolean</span></span>|<span data-ttu-id="fa7f2-120">リクエスターは、対象となるロールの割り当てのアクセス レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="fa7f2-120">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa7f2-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa7f2-121">JSON representation</span></span>

<span data-ttu-id="fa7f2-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa7f2-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
