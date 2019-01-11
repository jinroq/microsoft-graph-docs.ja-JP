---
title: Intune を使用して会社所有のデバイスを登録する
description: " (BYOD) のシナリオです。"
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07623c878ac3df9d8a171d7850868f2d7b84e56c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843940"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="89845-103">Intune を使用して会社所有のデバイスを登録する</span><span class="sxs-lookup"><span data-stu-id="89845-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="89845-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="89845-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89845-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89845-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89845-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="89845-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="89845-107">組織所有または会社所有のデバイスを登録して、デバイスの種類、デバイスの購入方法、組織のニーズに応じて、さまざまな方法で Intune で管理することができます。</span><span class="sxs-lookup"><span data-stu-id="89845-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="89845-108">また、ポータル サイト アプリをインストールして、会社所有のデバイスの登録と管理を、"Bring Your Own Device" (BYOD) のようなシナリオで行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="89845-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="89845-109">次の Graph リソースを使用して、Intune での会社所有のデバイスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="89845-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="89845-110">Active directory windows 自動操縦装置の配置のプロファイル</span><span class="sxs-lookup"><span data-stu-id="89845-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="89845-111">Azure AD windows 自動操縦装置の配置のプロファイル</span><span class="sxs-lookup"><span data-stu-id="89845-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="89845-112">DEP の登録の基本プロファイル</span><span class="sxs-lookup"><span data-stu-id="89845-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="89845-113">DEP 登録プロファイル</span><span class="sxs-lookup"><span data-stu-id="89845-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="89845-114">DEP iOS 登録プロファイル</span><span class="sxs-lookup"><span data-stu-id="89845-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="89845-115">DEP macOS 登録プロファイル</span><span class="sxs-lookup"><span data-stu-id="89845-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="89845-116">DEP の採用の設定</span><span class="sxs-lookup"><span data-stu-id="89845-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="89845-117">DEP のトークンの種類</span><span class="sxs-lookup"><span data-stu-id="89845-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="89845-118">法的証拠開示要求</span><span class="sxs-lookup"><span data-stu-id="89845-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="89845-119">登録プロファイル</span><span class="sxs-lookup"><span data-stu-id="89845-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="89845-120">登録状態</span><span class="sxs-lookup"><span data-stu-id="89845-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="89845-121">インポートされた Apple のデバイス id</span><span class="sxs-lookup"><span data-stu-id="89845-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="89845-122">Apple デバイス識別情報の結果のインポート</span><span class="sxs-lookup"><span data-stu-id="89845-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="89845-123">インポートされたデバイスの識別情報</span><span class="sxs-lookup"><span data-stu-id="89845-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="89845-124">デバイス識別情報の結果のインポート</span><span class="sxs-lookup"><span data-stu-id="89845-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="89845-125">デバイス id の種類をインポート</span><span class="sxs-lookup"><span data-stu-id="89845-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="89845-126">インポートされた windows の自動操縦装置のデバイス id</span><span class="sxs-lookup"><span data-stu-id="89845-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="89845-127">インポートされた windows 自動操縦装置のデバイス id のインポート状態</span><span class="sxs-lookup"><span data-stu-id="89845-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="89845-128">インポートされた windows 自動操縦装置のアイデンティティの状態</span><span class="sxs-lookup"><span data-stu-id="89845-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="89845-129">インポートされた windows 自動操縦装置のデバイス識別情報のアップロード</span><span class="sxs-lookup"><span data-stu-id="89845-129">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="89845-130">インポートされた windows 自動操縦装置のデバイス id アップロード状態</span><span class="sxs-lookup"><span data-stu-id="89845-130">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="89845-131">iTunes ペアリング モード</span><span class="sxs-lookup"><span data-stu-id="89845-131">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="89845-132">拇印を含む証明書を管理</span><span class="sxs-lookup"><span data-stu-id="89845-132">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="89845-133">ボックス エクスペリエンスの設定</span><span class="sxs-lookup"><span data-stu-id="89845-133">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="89845-134">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="89845-134">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="89845-135">Windows 自動操縦装置の配置のプロファイル</span><span class="sxs-lookup"><span data-stu-id="89845-135">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="89845-136">Windows 自動操縦装置の配置のプロファイル割り当て</span><span class="sxs-lookup"><span data-stu-id="89845-136">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="89845-137">Windows 自動操縦装置のデバイス id</span><span class="sxs-lookup"><span data-stu-id="89845-137">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="89845-138">Windows 自動操縦装置のプロファイルの割り当てステータスの詳細</span><span class="sxs-lookup"><span data-stu-id="89845-138">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="89845-139">Windows 自動操縦装置のプロファイルの割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="89845-139">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="89845-140">Windows の自動操縦装置の設定</span><span class="sxs-lookup"><span data-stu-id="89845-140">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="89845-141">Windows 自動操縦装置の同期の状態</span><span class="sxs-lookup"><span data-stu-id="89845-141">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="89845-142">Windows デバイスの使用法の種類</span><span class="sxs-lookup"><span data-stu-id="89845-142">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="89845-143">Windows の登録ステータス画面の設定</span><span class="sxs-lookup"><span data-stu-id="89845-143">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="89845-144">Windows ユーザーの種類</span><span class="sxs-lookup"><span data-stu-id="89845-144">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
