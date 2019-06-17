---
title: Binarymanagementconditionexpression 演算子 Type 列挙型
description: 管理条件式に対してサポートされる二項演算子。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b998bc9430a52347de255d9babfea8fd6061601d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994805"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="95267-103">Binarymanagementconditionexpression 演算子 Type 列挙型</span><span class="sxs-lookup"><span data-stu-id="95267-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="95267-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95267-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95267-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95267-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95267-106">管理条件式に対してサポートされる二項演算子。</span><span class="sxs-lookup"><span data-stu-id="95267-106">Supported binary operators for management condition expressions.</span></span>

## <a name="members"></a><span data-ttu-id="95267-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="95267-107">Members</span></span>
|<span data-ttu-id="95267-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="95267-108">Member</span></span>|<span data-ttu-id="95267-109">値</span><span class="sxs-lookup"><span data-stu-id="95267-109">Value</span></span>|<span data-ttu-id="95267-110">説明</span><span class="sxs-lookup"><span data-stu-id="95267-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95267-111">または</span><span class="sxs-lookup"><span data-stu-id="95267-111">or</span></span>|<span data-ttu-id="95267-112">.0</span><span class="sxs-lookup"><span data-stu-id="95267-112">0</span></span>|<span data-ttu-id="95267-113">オペランドが1つ以上 true の場合にのみ、オペランドのセットを true として評価します。</span><span class="sxs-lookup"><span data-stu-id="95267-113">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="95267-114">and</span><span class="sxs-lookup"><span data-stu-id="95267-114">and</span></span>|<span data-ttu-id="95267-115">1-d</span><span class="sxs-lookup"><span data-stu-id="95267-115">1</span></span>|<span data-ttu-id="95267-116">オペランドのセットを true として評価し、そのすべてのオペランドが true の場合にのみ評価します。</span><span class="sxs-lookup"><span data-stu-id="95267-116">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|





