---
title: WindowsPrivacyDataAccessControlItem を作成します。
description: 新しい windowsPrivacyDataAccessControlItem オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ec9aa9f4b8351c4f64ce468027f1f46e7d139a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948934"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="a1ae6-103">WindowsPrivacyDataAccessControlItem を作成します。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="a1ae6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1ae6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1ae6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1ae6-107">新しい[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1ae6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a1ae6-108">Prerequisites</span></span>
<span data-ttu-id="a1ae6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1ae6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1ae6-111">Permission type</span></span>|<span data-ttu-id="a1ae6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1ae6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1ae6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1ae6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1ae6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1ae6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1ae6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1ae6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1ae6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-116">Not supported.</span></span>|
|<span data-ttu-id="a1ae6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1ae6-117">Application</span></span>|<span data-ttu-id="a1ae6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1ae6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1ae6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="a1ae6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1ae6-120">Request headers</span></span>
|<span data-ttu-id="a1ae6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1ae6-121">Header</span></span>|<span data-ttu-id="a1ae6-122">値</span><span class="sxs-lookup"><span data-stu-id="a1ae6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1ae6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1ae6-123">Authorization</span></span>|<span data-ttu-id="a1ae6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1ae6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1ae6-125">Accept</span></span>|<span data-ttu-id="a1ae6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1ae6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1ae6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1ae6-127">Request body</span></span>
<span data-ttu-id="a1ae6-128">要求の本文に windowsPrivacyDataAccessControlItem オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="a1ae6-129">次の表は、windowsPrivacyDataAccessControlItem を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="a1ae6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1ae6-130">Property</span></span>|<span data-ttu-id="a1ae6-131">種類</span><span class="sxs-lookup"><span data-stu-id="a1ae6-131">Type</span></span>|<span data-ttu-id="a1ae6-132">説明</span><span class="sxs-lookup"><span data-stu-id="a1ae6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1ae6-133">ID</span><span class="sxs-lookup"><span data-stu-id="a1ae6-133">id</span></span>|<span data-ttu-id="a1ae6-134">String</span><span class="sxs-lookup"><span data-stu-id="a1ae6-134">String</span></span>|<span data-ttu-id="a1ae6-135">WindowsPrivacyDataAccessControlItem のキー。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="a1ae6-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="a1ae6-136">accessLevel</span></span>|[<span data-ttu-id="a1ae6-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="a1ae6-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="a1ae6-138">プライバシー データ カテゴリに、指定したアプリケーションを指定するアクセス レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="a1ae6-139">可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="a1ae6-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="a1ae6-140">dataCategory</span></span>|[<span data-ttu-id="a1ae6-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="a1ae6-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="a1ae6-142">これは、特定のアクセス制御が適用されるプライバシー データのカテゴリを示します。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="a1ae6-143">使用可能な値: `notConfigured`、 `accountInfo`、 `appsRunInBackground`、 `calendar`、 `callHistory`、 `camera`、 `contacts`、 `diagnosticsInfo`、 `email`、 `location`、 `messaging`、 `microphone`、 `motion`、 `notifications`、 `phone`、 `radios`、 `tasks`、 `syncWithDevices`、 `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="a1ae6-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="a1ae6-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="a1ae6-144">appPackageFamilyName</span></span>|<span data-ttu-id="a1ae6-145">String</span><span class="sxs-lookup"><span data-stu-id="a1ae6-145">String</span></span>|<span data-ttu-id="a1ae6-146">Windows アプリケーションのパッケージ ファミリ名です。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="a1ae6-147">アクセス レベルを設定すると、指定したアプリケーションを適用します。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="a1ae6-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1ae6-148">appDisplayName</span></span>|<span data-ttu-id="a1ae6-149">String</span><span class="sxs-lookup"><span data-stu-id="a1ae6-149">String</span></span>|<span data-ttu-id="a1ae6-150">Windows アプリケーションのパッケージ ファミリ名です。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="a1ae6-151">アクセス レベルを設定すると、指定したアプリケーションを適用します。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="a1ae6-152">応答</span><span class="sxs-lookup"><span data-stu-id="a1ae6-152">Response</span></span>
<span data-ttu-id="a1ae6-153">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1ae6-154">例</span><span class="sxs-lookup"><span data-stu-id="a1ae6-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1ae6-155">要求</span><span class="sxs-lookup"><span data-stu-id="a1ae6-155">Request</span></span>
<span data-ttu-id="a1ae6-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a1ae6-157">応答</span><span class="sxs-lookup"><span data-stu-id="a1ae6-157">Response</span></span>
<span data-ttu-id="a1ae6-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1ae6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "03b15556-5556-03b1-5655-b1035655b103",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```





