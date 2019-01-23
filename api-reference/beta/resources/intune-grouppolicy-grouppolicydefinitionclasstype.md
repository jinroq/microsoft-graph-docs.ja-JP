---
title: groupPolicyDefinitionClassType 列挙型
description: グループ ポリシーの定義のクラスの型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: afd1e6a8ebead5b0e81fe9d13351061ff20a96b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430522"
---
# <a name="grouppolicydefinitionclasstype-enum-type"></a><span data-ttu-id="c3ef1-103">groupPolicyDefinitionClassType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c3ef1-103">groupPolicyDefinitionClassType enum type</span></span>

> <span data-ttu-id="c3ef1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3ef1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c3ef1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3ef1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3ef1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3ef1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3ef1-107">グループ ポリシーの定義のクラスの型。</span><span class="sxs-lookup"><span data-stu-id="c3ef1-107">Group Policy Definition Class Type.</span></span>

## <a name="members"></a><span data-ttu-id="c3ef1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c3ef1-108">Members</span></span>
|<span data-ttu-id="c3ef1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c3ef1-109">Member</span></span>|<span data-ttu-id="c3ef1-110">値</span><span class="sxs-lookup"><span data-stu-id="c3ef1-110">Value</span></span>|<span data-ttu-id="c3ef1-111">説明</span><span class="sxs-lookup"><span data-stu-id="c3ef1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3ef1-112">user</span><span class="sxs-lookup"><span data-stu-id="c3ef1-112">user</span></span>|<span data-ttu-id="c3ef1-113">0</span><span class="sxs-lookup"><span data-stu-id="c3ef1-113">0</span></span>|<span data-ttu-id="c3ef1-114">[ユーザー構成] ノードは、ポリシー設定の位置を識別します。</span><span class="sxs-lookup"><span data-stu-id="c3ef1-114">Identifies placement of the policy setting under the user configuration node.</span></span>|
|<span data-ttu-id="c3ef1-115">マシン</span><span class="sxs-lookup"><span data-stu-id="c3ef1-115">machine</span></span>|<span data-ttu-id="c3ef1-116">1</span><span class="sxs-lookup"><span data-stu-id="c3ef1-116">1</span></span>|<span data-ttu-id="c3ef1-117">ポリシーの設定、コンピューターの構成] ノードの下の位置を識別します。</span><span class="sxs-lookup"><span data-stu-id="c3ef1-117">Identifies placement of the policy setting under the computer configuration node.</span></span>|
|<span data-ttu-id="c3ef1-118">両方とも</span><span class="sxs-lookup"><span data-stu-id="c3ef1-118">both</span></span>|<span data-ttu-id="c3ef1-119">2</span><span class="sxs-lookup"><span data-stu-id="c3ef1-119">2</span></span>|<span data-ttu-id="c3ef1-120">ポリシーの設定、コンピューターとユーザーの構成ノードの下の位置を識別します。</span><span class="sxs-lookup"><span data-stu-id="c3ef1-120">Identifies placement of the policy setting under both the computer and user configuration nodes.</span></span>|




