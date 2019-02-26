---
title: Intune を使用して会社のデバイスを登録する-Microsoft Graph API
description: テナント組織のデバイスを登録する Intune エンドポイント (REST) の Microsoft graph API の一覧を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 240bdc2d65d1ed8920fe1f9c067f1ffcd31a9f11
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149834"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="03f1b-103">Intune を使用して会社所有のデバイスを登録する</span><span class="sxs-lookup"><span data-stu-id="03f1b-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="03f1b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="03f1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03f1b-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03f1b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03f1b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="03f1b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="03f1b-107">組織所有または会社所有のデバイスを登録して、デバイスの種類、デバイスの購入方法、組織のニーズに応じて、さまざまな方法で Intune で管理することができます。</span><span class="sxs-lookup"><span data-stu-id="03f1b-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="03f1b-108">また、ポータル サイト アプリをインストールして、会社所有のデバイスの登録と管理を、"Bring Your Own Device" (BYOD) のようなシナリオで行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="03f1b-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="03f1b-109">次の Graph リソースを使用して、Intune での会社所有のデバイスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="03f1b-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="03f1b-110">Active Directory Windows Autopilot 展開プロファイル</span><span class="sxs-lookup"><span data-stu-id="03f1b-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="03f1b-111">Azure AD Windows Autopilot 展開プロファイル</span><span class="sxs-lookup"><span data-stu-id="03f1b-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="03f1b-112">DEP 登録ベース プロファイル</span><span class="sxs-lookup"><span data-stu-id="03f1b-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="03f1b-113">DEP 登録プロファイル</span><span class="sxs-lookup"><span data-stu-id="03f1b-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="03f1b-114">DEP iOS 登録プロファイル</span><span class="sxs-lookup"><span data-stu-id="03f1b-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="03f1b-115">DEP macOS 登録プロファイル</span><span class="sxs-lookup"><span data-stu-id="03f1b-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="03f1b-116">DEP オンボード設定</span><span class="sxs-lookup"><span data-stu-id="03f1b-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="03f1b-117">DEP トークンの種類</span><span class="sxs-lookup"><span data-stu-id="03f1b-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="03f1b-118">探索ソース</span><span class="sxs-lookup"><span data-stu-id="03f1b-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="03f1b-119">登録プロファイル</span><span class="sxs-lookup"><span data-stu-id="03f1b-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="03f1b-120">登録状態</span><span class="sxs-lookup"><span data-stu-id="03f1b-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="03f1b-121">インポートしたアップル デバイス ID</span><span class="sxs-lookup"><span data-stu-id="03f1b-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="03f1b-122">インポートしたアップル デバイス ID の結果</span><span class="sxs-lookup"><span data-stu-id="03f1b-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="03f1b-123">インポートしたデバイス ID </span><span class="sxs-lookup"><span data-stu-id="03f1b-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="03f1b-124">インポートしたデバイス ID の結果</span><span class="sxs-lookup"><span data-stu-id="03f1b-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="03f1b-125">インポートしたデバイス ID のタイプ</span><span class="sxs-lookup"><span data-stu-id="03f1b-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="03f1b-126">インポートした Windows AutoPilot デバイス ID</span><span class="sxs-lookup"><span data-stu-id="03f1b-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="03f1b-127">インポートした Windows AutoPilot デバイス ID のインポート状態</span><span class="sxs-lookup"><span data-stu-id="03f1b-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="03f1b-128">インポートした Windows AutoPilot デバイス ID の状態</span><span class="sxs-lookup"><span data-stu-id="03f1b-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="03f1b-129">インポートした Windows AutoPilot デバイス ID のアップロード</span><span class="sxs-lookup"><span data-stu-id="03f1b-129">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="03f1b-130">インポートした Windows AutoPilot デバイス ID のアップロードの状態</span><span class="sxs-lookup"><span data-stu-id="03f1b-130">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="03f1b-131">iTunes ペアリング モード</span><span class="sxs-lookup"><span data-stu-id="03f1b-131">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="03f1b-132">拇印を含む証明書の管理</span><span class="sxs-lookup"><span data-stu-id="03f1b-132">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="03f1b-133">Out Of Box Experience の設定</span><span class="sxs-lookup"><span data-stu-id="03f1b-133">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="03f1b-134">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="03f1b-134">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="03f1b-135">Windows Autopilot 展開プロファイル</span><span class="sxs-lookup"><span data-stu-id="03f1b-135">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="03f1b-136">Windows AutoPilot Deployment プロファイルの割り当て</span><span class="sxs-lookup"><span data-stu-id="03f1b-136">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="03f1b-137">Windows AutoPilot デバイス ID</span><span class="sxs-lookup"><span data-stu-id="03f1b-137">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="03f1b-138">Windows Autopilot プロファイルの割り当ての状態の詳細</span><span class="sxs-lookup"><span data-stu-id="03f1b-138">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="03f1b-139">Windows Autopilot プロファイルの割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="03f1b-139">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="03f1b-140">Windows Autopilot の設定</span><span class="sxs-lookup"><span data-stu-id="03f1b-140">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="03f1b-141">Windows AutoPilot の同期状態</span><span class="sxs-lookup"><span data-stu-id="03f1b-141">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="03f1b-142">Windows デバイスの使用法の種類</span><span class="sxs-lookup"><span data-stu-id="03f1b-142">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="03f1b-143">Windows 登録ステータス画面の設定</span><span class="sxs-lookup"><span data-stu-id="03f1b-143">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="03f1b-144">Windows ユーザーの種類</span><span class="sxs-lookup"><span data-stu-id="03f1b-144">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
