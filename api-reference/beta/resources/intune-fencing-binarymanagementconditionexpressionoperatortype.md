---
title: binarymanagementconditionexpression 演算子 type 列挙型
description: 管理条件式に対してサポートされる二項演算子。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35f60b9ee321ef3cbd65cf77273a65e7705f666a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143807"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="9f437-103">binarymanagementconditionexpression 演算子 type 列挙型</span><span class="sxs-lookup"><span data-stu-id="9f437-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="9f437-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f437-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f437-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f437-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f437-106">管理条件式に対してサポートされる二項演算子。</span><span class="sxs-lookup"><span data-stu-id="9f437-106">Supported binary operators for management condition expressions.</span></span>

## <a name="members"></a><span data-ttu-id="9f437-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9f437-107">Members</span></span>
|<span data-ttu-id="9f437-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9f437-108">Member</span></span>|<span data-ttu-id="9f437-109">値</span><span class="sxs-lookup"><span data-stu-id="9f437-109">Value</span></span>|<span data-ttu-id="9f437-110">説明</span><span class="sxs-lookup"><span data-stu-id="9f437-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f437-111">または</span><span class="sxs-lookup"><span data-stu-id="9f437-111">or</span></span>|<span data-ttu-id="9f437-112">.0</span><span class="sxs-lookup"><span data-stu-id="9f437-112">0</span></span>|<span data-ttu-id="9f437-113">オペランドが1つ以上 true の場合にのみ、オペランドのセットを true として評価します。</span><span class="sxs-lookup"><span data-stu-id="9f437-113">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="9f437-114">and</span><span class="sxs-lookup"><span data-stu-id="9f437-114">and</span></span>|<span data-ttu-id="9f437-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9f437-115">1</span></span>|<span data-ttu-id="9f437-116">オペランドのセットを true として評価し、そのすべてのオペランドが true の場合にのみ評価します。</span><span class="sxs-lookup"><span data-stu-id="9f437-116">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|




