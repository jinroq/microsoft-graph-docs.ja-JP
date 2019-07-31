---
title: Binarymanagementconditionexpression 演算子 Type 列挙型
description: 管理条件式に対してサポートされる二項演算子。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e885c1f04db2429869297e9022bf0e45f0f12e9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998738"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="1dfa2-103">Binarymanagementconditionexpression 演算子 Type 列挙型</span><span class="sxs-lookup"><span data-stu-id="1dfa2-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="1dfa2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dfa2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dfa2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1dfa2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dfa2-106">管理条件式に対してサポートされる二項演算子。</span><span class="sxs-lookup"><span data-stu-id="1dfa2-106">Supported binary operators for management condition expressions.</span></span>

## <a name="members"></a><span data-ttu-id="1dfa2-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1dfa2-107">Members</span></span>
|<span data-ttu-id="1dfa2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1dfa2-108">Member</span></span>|<span data-ttu-id="1dfa2-109">値</span><span class="sxs-lookup"><span data-stu-id="1dfa2-109">Value</span></span>|<span data-ttu-id="1dfa2-110">説明</span><span class="sxs-lookup"><span data-stu-id="1dfa2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dfa2-111">または</span><span class="sxs-lookup"><span data-stu-id="1dfa2-111">or</span></span>|<span data-ttu-id="1dfa2-112">.0</span><span class="sxs-lookup"><span data-stu-id="1dfa2-112">0</span></span>|<span data-ttu-id="1dfa2-113">オペランドが1つ以上 true の場合にのみ、オペランドのセットを true として評価します。</span><span class="sxs-lookup"><span data-stu-id="1dfa2-113">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="1dfa2-114">and</span><span class="sxs-lookup"><span data-stu-id="1dfa2-114">and</span></span>|<span data-ttu-id="1dfa2-115">1-d</span><span class="sxs-lookup"><span data-stu-id="1dfa2-115">1</span></span>|<span data-ttu-id="1dfa2-116">オペランドのセットを true として評価し、そのすべてのオペランドが true の場合にのみ評価します。</span><span class="sxs-lookup"><span data-stu-id="1dfa2-116">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|





