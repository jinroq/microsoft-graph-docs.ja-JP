---
title: WindowsAssignedAccessProfile を更新します。
description: WindowsAssignedAccessProfile オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 84cbc1aaaebf9383c3d113d7f309c61de0cdeb67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331361"
---
# <a name="update-windowsassignedaccessprofile"></a><span data-ttu-id="9d35d-103">WindowsAssignedAccessProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="9d35d-103">Update windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="9d35d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d35d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d35d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d35d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d35d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d35d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d35d-107">[WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9d35d-107">Update the properties of a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d35d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9d35d-108">Prerequisites</span></span>
<span data-ttu-id="9d35d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d35d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d35d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d35d-111">Permission type</span></span>|<span data-ttu-id="9d35d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d35d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d35d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d35d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d35d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d35d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d35d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d35d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d35d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d35d-116">Not supported.</span></span>|
|<span data-ttu-id="9d35d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d35d-117">Application</span></span>|<span data-ttu-id="9d35d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d35d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d35d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d35d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="9d35d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d35d-120">Request headers</span></span>
|<span data-ttu-id="9d35d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d35d-121">Header</span></span>|<span data-ttu-id="9d35d-122">値</span><span class="sxs-lookup"><span data-stu-id="9d35d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d35d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d35d-123">Authorization</span></span>|<span data-ttu-id="9d35d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9d35d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d35d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d35d-125">Accept</span></span>|<span data-ttu-id="9d35d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d35d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d35d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d35d-127">Request body</span></span>
<span data-ttu-id="9d35d-128">要求の本文に[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d35d-128">In the request body, supply a JSON representation for the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>

<span data-ttu-id="9d35d-129">[WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="9d35d-129">The following table shows the properties that are required when you create the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span></span>

|<span data-ttu-id="9d35d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d35d-130">Property</span></span>|<span data-ttu-id="9d35d-131">種類</span><span class="sxs-lookup"><span data-stu-id="9d35d-131">Type</span></span>|<span data-ttu-id="9d35d-132">説明</span><span class="sxs-lookup"><span data-stu-id="9d35d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d35d-133">ID</span><span class="sxs-lookup"><span data-stu-id="9d35d-133">id</span></span>|<span data-ttu-id="9d35d-134">String</span><span class="sxs-lookup"><span data-stu-id="9d35d-134">String</span></span>|<span data-ttu-id="9d35d-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9d35d-135">Key of the entity.</span></span>|
|<span data-ttu-id="9d35d-136">profilename プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d35d-136">profileName</span></span>|<span data-ttu-id="9d35d-137">String</span><span class="sxs-lookup"><span data-stu-id="9d35d-137">String</span></span>|<span data-ttu-id="9d35d-138">これは、[スタート] メニューの [このプレゼンテーションの構成が割り当てられているユーザーにこれらのアプリケーションのレイアウト、アプリケーションのグループを識別するために使用するフレンドリ名です。</span><span class="sxs-lookup"><span data-stu-id="9d35d-138">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="9d35d-139">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="9d35d-139">showTaskBar</span></span>|<span data-ttu-id="9d35d-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="9d35d-140">Boolean</span></span>|<span data-ttu-id="9d35d-141">この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。</span><span class="sxs-lookup"><span data-stu-id="9d35d-141">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="9d35d-142">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="9d35d-142">appUserModelIds</span></span>|<span data-ttu-id="9d35d-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9d35d-143">String collection</span></span>|<span data-ttu-id="9d35d-144">これらは、[スタート] メニューから起動できる唯一の Windows ストア アプリです。</span><span class="sxs-lookup"><span data-stu-id="9d35d-144">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="9d35d-145">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="9d35d-145">desktopAppPaths</span></span>|<span data-ttu-id="9d35d-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9d35d-146">String collection</span></span>|<span data-ttu-id="9d35d-147">これらは、[スタート] メニューで利用可能なデスクトップ アプリケーションのパスと、唯一のアプリケーション、ユーザーが起動できるようです。</span><span class="sxs-lookup"><span data-stu-id="9d35d-147">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="9d35d-148">ユーザー アカウント</span><span class="sxs-lookup"><span data-stu-id="9d35d-148">userAccounts</span></span>|<span data-ttu-id="9d35d-149">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9d35d-149">String collection</span></span>|<span data-ttu-id="9d35d-150">この構成にキオスクがロックアウトされているユーザー アカウントです。</span><span class="sxs-lookup"><span data-stu-id="9d35d-150">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="9d35d-151">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="9d35d-151">startMenuLayoutXml</span></span>|<span data-ttu-id="9d35d-152">Binary</span><span class="sxs-lookup"><span data-stu-id="9d35d-152">Binary</span></span>|<span data-ttu-id="9d35d-153">開始の既定のレイアウトを変更するのには管理者は、ユーザーが変更できないようにします。</span><span class="sxs-lookup"><span data-stu-id="9d35d-153">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="9d35d-154">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="9d35d-154"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="9d35d-155">XML は、バイナリ形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d35d-155">XML needs to be in Binary format.</span></span>|



## <a name="response"></a><span data-ttu-id="9d35d-156">応答</span><span class="sxs-lookup"><span data-stu-id="9d35d-156">Response</span></span>
<span data-ttu-id="9d35d-157">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9d35d-157">If successful, this method returns a `200 OK` response code and an updated [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d35d-158">例</span><span class="sxs-lookup"><span data-stu-id="9d35d-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d35d-159">要求</span><span class="sxs-lookup"><span data-stu-id="9d35d-159">Request</span></span>
<span data-ttu-id="9d35d-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9d35d-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d35d-161">応答</span><span class="sxs-lookup"><span data-stu-id="9d35d-161">Response</span></span>
<span data-ttu-id="9d35d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d35d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




