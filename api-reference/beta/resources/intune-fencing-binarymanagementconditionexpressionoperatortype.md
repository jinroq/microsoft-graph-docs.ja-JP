---
title: binaryManagementConditionExpressionOperatorType 列挙型
description: 管理条件式の二項演算子をサポートします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 141238fd90b6cae65ac50745d950d3d9d149280d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959413"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="5172c-103">binaryManagementConditionExpressionOperatorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5172c-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="5172c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5172c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5172c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5172c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5172c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5172c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5172c-107">管理条件式の二項演算子をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5172c-107">Supported binary operators for management condition expressions.</span></span>
## <a name="members"></a><span data-ttu-id="5172c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5172c-108">Members</span></span>
|<span data-ttu-id="5172c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5172c-109">Member</span></span>|<span data-ttu-id="5172c-110">値</span><span class="sxs-lookup"><span data-stu-id="5172c-110">Value</span></span>|<span data-ttu-id="5172c-111">説明</span><span class="sxs-lookup"><span data-stu-id="5172c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5172c-112">または</span><span class="sxs-lookup"><span data-stu-id="5172c-112">or</span></span>|<span data-ttu-id="5172c-113">0</span><span class="sxs-lookup"><span data-stu-id="5172c-113">0</span></span>|<span data-ttu-id="5172c-114">1 つ以上のオペランドが true の場合にのみ一連のオペランドが true と評価されました。</span><span class="sxs-lookup"><span data-stu-id="5172c-114">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="5172c-115">and</span><span class="sxs-lookup"><span data-stu-id="5172c-115">and</span></span>|<span data-ttu-id="5172c-116">1</span><span class="sxs-lookup"><span data-stu-id="5172c-116">1</span></span>|<span data-ttu-id="5172c-117">オペランドのすべてに該当する場合にのみ一連のオペランドが true と評価されました。</span><span class="sxs-lookup"><span data-stu-id="5172c-117">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|





