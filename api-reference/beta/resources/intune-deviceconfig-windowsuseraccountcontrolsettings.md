---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザーアカウント制御設定に指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8302566eea465ec4477a01845778ab2d7ddee9fe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146712"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="81974-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="81974-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="81974-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81974-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81974-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="81974-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81974-106">Windows ユーザーアカウント制御設定に指定できる値。</span><span class="sxs-lookup"><span data-stu-id="81974-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="81974-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="81974-107">Members</span></span>
|<span data-ttu-id="81974-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="81974-108">Member</span></span>|<span data-ttu-id="81974-109">値</span><span class="sxs-lookup"><span data-stu-id="81974-109">Value</span></span>|<span data-ttu-id="81974-110">説明</span><span class="sxs-lookup"><span data-stu-id="81974-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81974-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="81974-111">userDefined</span></span>|<span data-ttu-id="81974-112">.0</span><span class="sxs-lookup"><span data-stu-id="81974-112">0</span></span>|<span data-ttu-id="81974-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="81974-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="81974-114">常に通知</span><span class="sxs-lookup"><span data-stu-id="81974-114">alwaysNotify</span></span>|<span data-ttu-id="81974-115">1-d</span><span class="sxs-lookup"><span data-stu-id="81974-115">1</span></span>|<span data-ttu-id="81974-116">常に通知します。</span><span class="sxs-lookup"><span data-stu-id="81974-116">Always notify.</span></span>|
|<span data-ttu-id="81974-117">notifyonappchanges</span><span class="sxs-lookup"><span data-stu-id="81974-117">notifyOnAppChanges</span></span>|<span data-ttu-id="81974-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="81974-118">2</span></span>|<span data-ttu-id="81974-119">アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="81974-119">Notify on app changes.</span></span>|
|<span data-ttu-id="81974-120">notifyonappのすべての非追加暗転</span><span class="sxs-lookup"><span data-stu-id="81974-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="81974-121">1/3</span><span class="sxs-lookup"><span data-stu-id="81974-121">3</span></span>|<span data-ttu-id="81974-122">デスクトップを暗転せずに、アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="81974-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="81974-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="81974-123">neverNotify</span></span>|<span data-ttu-id="81974-124">2/4</span><span class="sxs-lookup"><span data-stu-id="81974-124">4</span></span>|<span data-ttu-id="81974-125">通知しません。</span><span class="sxs-lookup"><span data-stu-id="81974-125">Never notify.</span></span>|




