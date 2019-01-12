---
title: WindowsAssignedAccessProfile を更新します。
description: WindowsAssignedAccessProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f82a1ad5a5bdea639ec3dc24f40a3c66c4a0fe1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940380"
---
# <a name="update-windowsassignedaccessprofile"></a><span data-ttu-id="1e695-103">WindowsAssignedAccessProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="1e695-103">Update windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="1e695-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e695-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e695-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e695-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e695-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e695-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e695-107">[WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1e695-107">Update the properties of a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e695-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1e695-108">Prerequisites</span></span>
<span data-ttu-id="1e695-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e695-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e695-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e695-111">Permission type</span></span>|<span data-ttu-id="1e695-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e695-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e695-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e695-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e695-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e695-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e695-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e695-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e695-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e695-116">Not supported.</span></span>|
|<span data-ttu-id="1e695-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e695-117">Application</span></span>|<span data-ttu-id="1e695-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e695-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e695-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e695-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="1e695-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e695-120">Request headers</span></span>
|<span data-ttu-id="1e695-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e695-121">Header</span></span>|<span data-ttu-id="1e695-122">値</span><span class="sxs-lookup"><span data-stu-id="1e695-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e695-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e695-123">Authorization</span></span>|<span data-ttu-id="1e695-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1e695-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e695-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e695-125">Accept</span></span>|<span data-ttu-id="1e695-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e695-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e695-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e695-127">Request body</span></span>
<span data-ttu-id="1e695-128">要求の本文に[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e695-128">In the request body, supply a JSON representation for the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>

<span data-ttu-id="1e695-129">[WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="1e695-129">The following table shows the properties that are required when you create the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span></span>

|<span data-ttu-id="1e695-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e695-130">Property</span></span>|<span data-ttu-id="1e695-131">型</span><span class="sxs-lookup"><span data-stu-id="1e695-131">Type</span></span>|<span data-ttu-id="1e695-132">説明</span><span class="sxs-lookup"><span data-stu-id="1e695-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e695-133">ID</span><span class="sxs-lookup"><span data-stu-id="1e695-133">id</span></span>|<span data-ttu-id="1e695-134">String</span><span class="sxs-lookup"><span data-stu-id="1e695-134">String</span></span>|<span data-ttu-id="1e695-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1e695-135">Key of the entity.</span></span>|
|<span data-ttu-id="1e695-136">profilename プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e695-136">profileName</span></span>|<span data-ttu-id="1e695-137">String</span><span class="sxs-lookup"><span data-stu-id="1e695-137">String</span></span>|<span data-ttu-id="1e695-138">これは、[スタート] メニューの [このプレゼンテーションの構成が割り当てられているユーザーにこれらのアプリケーションのレイアウト、アプリケーションのグループを識別するために使用するフレンドリ名です。</span><span class="sxs-lookup"><span data-stu-id="1e695-138">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="1e695-139">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="1e695-139">showTaskBar</span></span>|<span data-ttu-id="1e695-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e695-140">Boolean</span></span>|<span data-ttu-id="1e695-141">この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。</span><span class="sxs-lookup"><span data-stu-id="1e695-141">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="1e695-142">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="1e695-142">appUserModelIds</span></span>|<span data-ttu-id="1e695-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1e695-143">String collection</span></span>|<span data-ttu-id="1e695-144">これらは、[スタート] メニューから起動できる唯一の Windows ストア アプリです。</span><span class="sxs-lookup"><span data-stu-id="1e695-144">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="1e695-145">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="1e695-145">desktopAppPaths</span></span>|<span data-ttu-id="1e695-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1e695-146">String collection</span></span>|<span data-ttu-id="1e695-147">これらは、[スタート] メニューで利用可能なデスクトップ アプリケーションのパスと、唯一のアプリケーション、ユーザーが起動できるようです。</span><span class="sxs-lookup"><span data-stu-id="1e695-147">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="1e695-148">ユーザー アカウント</span><span class="sxs-lookup"><span data-stu-id="1e695-148">userAccounts</span></span>|<span data-ttu-id="1e695-149">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1e695-149">String collection</span></span>|<span data-ttu-id="1e695-150">この構成にキオスクがロックアウトされているユーザー アカウントです。</span><span class="sxs-lookup"><span data-stu-id="1e695-150">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="1e695-151">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="1e695-151">startMenuLayoutXml</span></span>|<span data-ttu-id="1e695-152">Binary</span><span class="sxs-lookup"><span data-stu-id="1e695-152">Binary</span></span>|<span data-ttu-id="1e695-153">開始の既定のレイアウトを変更するのには管理者は、ユーザーが変更できないようにします。</span><span class="sxs-lookup"><span data-stu-id="1e695-153">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="1e695-154">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="1e695-154"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="1e695-155">XML は、バイナリ形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e695-155">XML needs to be in Binary format.</span></span>|



## <a name="response"></a><span data-ttu-id="1e695-156">応答</span><span class="sxs-lookup"><span data-stu-id="1e695-156">Response</span></span>
<span data-ttu-id="1e695-157">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1e695-157">If successful, this method returns a `200 OK` response code and an updated [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e695-158">例</span><span class="sxs-lookup"><span data-stu-id="1e695-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e695-159">要求</span><span class="sxs-lookup"><span data-stu-id="1e695-159">Request</span></span>
<span data-ttu-id="1e695-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e695-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
Content-type: application/json
Content-length: 297

{
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```

### <a name="response"></a><span data-ttu-id="1e695-161">応答</span><span class="sxs-lookup"><span data-stu-id="1e695-161">Response</span></span>
<span data-ttu-id="1e695-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1e695-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 413

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```





