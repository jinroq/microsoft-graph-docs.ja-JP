---
title: binaryManagementConditionExpressionOperatorType 列挙型
description: 管理条件式の二項演算子をサポートします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05b195df95d6f7a85673a352edf090cea7f074aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424295"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="65e02-103">binaryManagementConditionExpressionOperatorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="65e02-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="65e02-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65e02-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="65e02-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65e02-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65e02-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65e02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65e02-107">管理条件式の二項演算子をサポートします。</span><span class="sxs-lookup"><span data-stu-id="65e02-107">Supported binary operators for management condition expressions.</span></span>

## <a name="members"></a><span data-ttu-id="65e02-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="65e02-108">Members</span></span>
|<span data-ttu-id="65e02-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="65e02-109">Member</span></span>|<span data-ttu-id="65e02-110">値</span><span class="sxs-lookup"><span data-stu-id="65e02-110">Value</span></span>|<span data-ttu-id="65e02-111">説明</span><span class="sxs-lookup"><span data-stu-id="65e02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65e02-112">または</span><span class="sxs-lookup"><span data-stu-id="65e02-112">or</span></span>|<span data-ttu-id="65e02-113">0</span><span class="sxs-lookup"><span data-stu-id="65e02-113">0</span></span>|<span data-ttu-id="65e02-114">1 つ以上のオペランドが true の場合にのみ一連のオペランドが true と評価されました。</span><span class="sxs-lookup"><span data-stu-id="65e02-114">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="65e02-115">and</span><span class="sxs-lookup"><span data-stu-id="65e02-115">and</span></span>|<span data-ttu-id="65e02-116">1</span><span class="sxs-lookup"><span data-stu-id="65e02-116">1</span></span>|<span data-ttu-id="65e02-117">オペランドのすべてに該当する場合にのみ一連のオペランドが true と評価されました。</span><span class="sxs-lookup"><span data-stu-id="65e02-117">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|




