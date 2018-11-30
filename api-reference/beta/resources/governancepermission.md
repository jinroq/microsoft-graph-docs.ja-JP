---
title: governancePermission リソースの種類
description: '特定の governanceResource に、governanceSubject を持つアクセス許可を表します。  '
ms.openlocfilehash: d7b3e1eb70c89c278ccc2a8b3e9a16e265e4ae97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071072"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="0de57-103">governancePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0de57-103">governancePermission resource type</span></span>

> <span data-ttu-id="0de57-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0de57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0de57-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0de57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0de57-106">特定の[governanceResource](../resources/governanceresource.md)に、 [governanceSubject](../resources/governancesubject.md)を持つアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="0de57-106">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="0de57-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0de57-107">Properties</span></span>
| <span data-ttu-id="0de57-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0de57-108">Property</span></span>     | <span data-ttu-id="0de57-109">型</span><span class="sxs-lookup"><span data-stu-id="0de57-109">Type</span></span>   |<span data-ttu-id="0de57-110">説明</span><span class="sxs-lookup"><span data-stu-id="0de57-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0de57-111">accessLevel</span><span class="sxs-lookup"><span data-stu-id="0de57-111">accessLevel</span></span>|<span data-ttu-id="0de57-112">String</span><span class="sxs-lookup"><span data-stu-id="0de57-112">String</span></span>|<span data-ttu-id="0de57-113">アクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="0de57-113">The access level.</span></span> <span data-ttu-id="0de57-114">有効な値: ``None``、 ``UserRead``、``AdminRead``と``AdminReadWrite``。</span><span class="sxs-lookup"><span data-stu-id="0de57-114">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="0de57-115">isActive</span><span class="sxs-lookup"><span data-stu-id="0de57-115">isActive</span></span>|<span data-ttu-id="0de57-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="0de57-116">Boolean</span></span>|<span data-ttu-id="0de57-117">指定する場合、リクエスターが、アクティブなロールの割り当てのアクセス レベルを持ちます。</span><span class="sxs-lookup"><span data-stu-id="0de57-117">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="0de57-118">isEligible</span><span class="sxs-lookup"><span data-stu-id="0de57-118">isEligible</span></span>|<span data-ttu-id="0de57-119">ブール値</span><span class="sxs-lookup"><span data-stu-id="0de57-119">Boolean</span></span>|<span data-ttu-id="0de57-120">リクエスターは、対象となるロールの割り当てのアクセス レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="0de57-120">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0de57-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0de57-121">JSON representation</span></span>

<span data-ttu-id="0de57-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0de57-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```