---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザーアカウント制御設定に指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a3183e2f8c7521474dfb2910eb5e6f5fbe6de14
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978662"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="657b2-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="657b2-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="657b2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="657b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="657b2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="657b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="657b2-106">Windows ユーザーアカウント制御設定に指定できる値。</span><span class="sxs-lookup"><span data-stu-id="657b2-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="657b2-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="657b2-107">Members</span></span>
|<span data-ttu-id="657b2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="657b2-108">Member</span></span>|<span data-ttu-id="657b2-109">値</span><span class="sxs-lookup"><span data-stu-id="657b2-109">Value</span></span>|<span data-ttu-id="657b2-110">説明</span><span class="sxs-lookup"><span data-stu-id="657b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="657b2-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="657b2-111">userDefined</span></span>|<span data-ttu-id="657b2-112">.0</span><span class="sxs-lookup"><span data-stu-id="657b2-112">0</span></span>|<span data-ttu-id="657b2-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="657b2-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="657b2-114">常に通知</span><span class="sxs-lookup"><span data-stu-id="657b2-114">alwaysNotify</span></span>|<span data-ttu-id="657b2-115">1-d</span><span class="sxs-lookup"><span data-stu-id="657b2-115">1</span></span>|<span data-ttu-id="657b2-116">常に通知します。</span><span class="sxs-lookup"><span data-stu-id="657b2-116">Always notify.</span></span>|
|<span data-ttu-id="657b2-117">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="657b2-117">notifyOnAppChanges</span></span>|<span data-ttu-id="657b2-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="657b2-118">2</span></span>|<span data-ttu-id="657b2-119">アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="657b2-119">Notify on app changes.</span></span>|
|<span data-ttu-id="657b2-120">Notifyonappのすべての非追加暗転</span><span class="sxs-lookup"><span data-stu-id="657b2-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="657b2-121">1/3</span><span class="sxs-lookup"><span data-stu-id="657b2-121">3</span></span>|<span data-ttu-id="657b2-122">デスクトップを暗転せずに、アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="657b2-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="657b2-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="657b2-123">neverNotify</span></span>|<span data-ttu-id="657b2-124">2/4</span><span class="sxs-lookup"><span data-stu-id="657b2-124">4</span></span>|<span data-ttu-id="657b2-125">通知しません。</span><span class="sxs-lookup"><span data-stu-id="657b2-125">Never notify.</span></span>|





