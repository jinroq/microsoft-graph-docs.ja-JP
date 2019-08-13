---
title: managedAppRemediationAction 列挙型
description: 管理対象アプリで適用される管理者が開始したアクション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ea9262766b281810f12beca67fab326fc517bc2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373288"
---
# <a name="managedappremediationaction-enum-type"></a><span data-ttu-id="c9613-103">managedAppRemediationAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="c9613-103">managedAppRemediationAction enum type</span></span>

> <span data-ttu-id="c9613-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9613-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9613-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9613-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9613-106">管理対象アプリで適用される管理者が開始したアクション。</span><span class="sxs-lookup"><span data-stu-id="c9613-106">An admin initiated action to be applied on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="c9613-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c9613-107">Members</span></span>
|<span data-ttu-id="c9613-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c9613-108">Member</span></span>|<span data-ttu-id="c9613-109">値</span><span class="sxs-lookup"><span data-stu-id="c9613-109">Value</span></span>|<span data-ttu-id="c9613-110">説明</span><span class="sxs-lookup"><span data-stu-id="c9613-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9613-111">拒否</span><span class="sxs-lookup"><span data-stu-id="c9613-111">block</span></span>|<span data-ttu-id="c9613-112">.0</span><span class="sxs-lookup"><span data-stu-id="c9613-112">0</span></span>|<span data-ttu-id="c9613-113">アプリと、ブロックされる対応会社のデータ</span><span class="sxs-lookup"><span data-stu-id="c9613-113">app and the corresponding company data to be blocked</span></span>|
|<span data-ttu-id="c9613-114">ふき</span><span class="sxs-lookup"><span data-stu-id="c9613-114">wipe</span></span>|<span data-ttu-id="c9613-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c9613-115">1</span></span>|<span data-ttu-id="c9613-116">消去するアプリと対応する会社のデータ</span><span class="sxs-lookup"><span data-stu-id="c9613-116">app and the corresponding company data to be wiped</span></span>|
|<span data-ttu-id="c9613-117">示す</span><span class="sxs-lookup"><span data-stu-id="c9613-117">warn</span></span>|<span data-ttu-id="c9613-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c9613-118">2</span></span>|<span data-ttu-id="c9613-119">警告対象のアプリと対応するユーザー</span><span class="sxs-lookup"><span data-stu-id="c9613-119">app and the corresponding user to be warned</span></span>|



