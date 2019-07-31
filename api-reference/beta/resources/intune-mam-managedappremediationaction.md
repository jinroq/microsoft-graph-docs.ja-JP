---
title: managedAppRemediationAction 列挙型
description: 管理対象アプリで適用される管理者が開始したアクション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d935845019e8d90e9f88246bd5c60699b5265e7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967939"
---
# <a name="managedappremediationaction-enum-type"></a><span data-ttu-id="3bb58-103">managedAppRemediationAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="3bb58-103">managedAppRemediationAction enum type</span></span>

> <span data-ttu-id="3bb58-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bb58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bb58-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3bb58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bb58-106">管理対象アプリで適用される管理者が開始したアクション。</span><span class="sxs-lookup"><span data-stu-id="3bb58-106">An admin initiated action to be applied on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="3bb58-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3bb58-107">Members</span></span>
|<span data-ttu-id="3bb58-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3bb58-108">Member</span></span>|<span data-ttu-id="3bb58-109">値</span><span class="sxs-lookup"><span data-stu-id="3bb58-109">Value</span></span>|<span data-ttu-id="3bb58-110">説明</span><span class="sxs-lookup"><span data-stu-id="3bb58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bb58-111">拒否</span><span class="sxs-lookup"><span data-stu-id="3bb58-111">block</span></span>|<span data-ttu-id="3bb58-112">.0</span><span class="sxs-lookup"><span data-stu-id="3bb58-112">0</span></span>|<span data-ttu-id="3bb58-113">アプリと、ブロックされる対応会社のデータ</span><span class="sxs-lookup"><span data-stu-id="3bb58-113">app and the corresponding company data to be blocked</span></span>|
|<span data-ttu-id="3bb58-114">ふき</span><span class="sxs-lookup"><span data-stu-id="3bb58-114">wipe</span></span>|<span data-ttu-id="3bb58-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3bb58-115">1</span></span>|<span data-ttu-id="3bb58-116">消去するアプリと対応する会社のデータ</span><span class="sxs-lookup"><span data-stu-id="3bb58-116">app and the corresponding company data to be wiped</span></span>|
|<span data-ttu-id="3bb58-117">示す</span><span class="sxs-lookup"><span data-stu-id="3bb58-117">warn</span></span>|<span data-ttu-id="3bb58-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3bb58-118">2</span></span>|<span data-ttu-id="3bb58-119">警告対象のアプリと対応するユーザー</span><span class="sxs-lookup"><span data-stu-id="3bb58-119">app and the corresponding user to be warned</span></span>|





