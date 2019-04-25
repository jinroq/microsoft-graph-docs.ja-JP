---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザーアカウント制御設定に指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b63fe44abfb0a06e5978d78e49c392c08122e38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523561"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="5c3a5-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="5c3a5-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="5c3a5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c3a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c3a5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c3a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c3a5-106">Windows ユーザーアカウント制御設定に指定できる値。</span><span class="sxs-lookup"><span data-stu-id="5c3a5-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="5c3a5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5c3a5-107">Members</span></span>
|<span data-ttu-id="5c3a5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5c3a5-108">Member</span></span>|<span data-ttu-id="5c3a5-109">値</span><span class="sxs-lookup"><span data-stu-id="5c3a5-109">Value</span></span>|<span data-ttu-id="5c3a5-110">説明</span><span class="sxs-lookup"><span data-stu-id="5c3a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c3a5-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="5c3a5-111">userDefined</span></span>|<span data-ttu-id="5c3a5-112">.0</span><span class="sxs-lookup"><span data-stu-id="5c3a5-112">0</span></span>|<span data-ttu-id="5c3a5-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="5c3a5-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5c3a5-114">常に通知</span><span class="sxs-lookup"><span data-stu-id="5c3a5-114">alwaysNotify</span></span>|<span data-ttu-id="5c3a5-115">1 </span><span class="sxs-lookup"><span data-stu-id="5c3a5-115">1</span></span>|<span data-ttu-id="5c3a5-116">常に通知します。</span><span class="sxs-lookup"><span data-stu-id="5c3a5-116">Always notify.</span></span>|
|<span data-ttu-id="5c3a5-117">notifyonappchanges</span><span class="sxs-lookup"><span data-stu-id="5c3a5-117">notifyOnAppChanges</span></span>|<span data-ttu-id="5c3a5-118">2 </span><span class="sxs-lookup"><span data-stu-id="5c3a5-118">2</span></span>|<span data-ttu-id="5c3a5-119">アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="5c3a5-119">Notify on app changes.</span></span>|
|<span data-ttu-id="5c3a5-120">notifyonappのすべての非追加暗転</span><span class="sxs-lookup"><span data-stu-id="5c3a5-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="5c3a5-121">3 </span><span class="sxs-lookup"><span data-stu-id="5c3a5-121">3</span></span>|<span data-ttu-id="5c3a5-122">デスクトップを暗転せずに、アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="5c3a5-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="5c3a5-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="5c3a5-123">neverNotify</span></span>|<span data-ttu-id="5c3a5-124">4 </span><span class="sxs-lookup"><span data-stu-id="5c3a5-124">4</span></span>|<span data-ttu-id="5c3a5-125">通知しません。</span><span class="sxs-lookup"><span data-stu-id="5c3a5-125">Never notify.</span></span>|





