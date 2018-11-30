---
title: WindowsPrivacyDataAccessControlItem を作成します。
description: 新しい windowsPrivacyDataAccessControlItem オブジェクトを作成します。
ms.openlocfilehash: 6466e4ddc0db738c30111e1ca836c60e5ec885ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072117"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="7f628-103">WindowsPrivacyDataAccessControlItem を作成します。</span><span class="sxs-lookup"><span data-stu-id="7f628-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="7f628-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f628-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f628-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f628-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f628-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f628-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f628-107">新しい[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7f628-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f628-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f628-108">Prerequisites</span></span>
<span data-ttu-id="7f628-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f628-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f628-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f628-111">Permission type</span></span>|<span data-ttu-id="7f628-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f628-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f628-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f628-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f628-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f628-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f628-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f628-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f628-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f628-116">Not supported.</span></span>|
|<span data-ttu-id="7f628-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f628-117">Application</span></span>|<span data-ttu-id="7f628-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f628-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f628-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f628-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="7f628-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f628-120">Request headers</span></span>
|<span data-ttu-id="7f628-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f628-121">Header</span></span>|<span data-ttu-id="7f628-122">値</span><span class="sxs-lookup"><span data-stu-id="7f628-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f628-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f628-123">Authorization</span></span>|<span data-ttu-id="7f628-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7f628-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f628-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f628-125">Accept</span></span>|<span data-ttu-id="7f628-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f628-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f628-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f628-127">Request body</span></span>
<span data-ttu-id="7f628-128">要求の本文に windowsPrivacyDataAccessControlItem オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f628-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="7f628-129">次の表は、windowsPrivacyDataAccessControlItem を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f628-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="7f628-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f628-130">Property</span></span>|<span data-ttu-id="7f628-131">型</span><span class="sxs-lookup"><span data-stu-id="7f628-131">Type</span></span>|<span data-ttu-id="7f628-132">説明</span><span class="sxs-lookup"><span data-stu-id="7f628-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f628-133">id</span><span class="sxs-lookup"><span data-stu-id="7f628-133">id</span></span>|<span data-ttu-id="7f628-134">String</span><span class="sxs-lookup"><span data-stu-id="7f628-134">String</span></span>|<span data-ttu-id="7f628-135">WindowsPrivacyDataAccessControlItem のキー。</span><span class="sxs-lookup"><span data-stu-id="7f628-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="7f628-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="7f628-136">accessLevel</span></span>|[<span data-ttu-id="7f628-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="7f628-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="7f628-138">プライバシー データ カテゴリに、指定したアプリケーションを指定するアクセス レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="7f628-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="7f628-139">可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。</span><span class="sxs-lookup"><span data-stu-id="7f628-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="7f628-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="7f628-140">dataCategory</span></span>|[<span data-ttu-id="7f628-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="7f628-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="7f628-142">これは、特定のアクセス制御が適用されるプライバシー データのカテゴリを示します。</span><span class="sxs-lookup"><span data-stu-id="7f628-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="7f628-143">使用可能な値: `notConfigured`、 `accountInfo`、 `appsRunInBackground`、 `calendar`、 `callHistory`、 `camera`、 `contacts`、 `diagnosticsInfo`、 `email`、 `location`、 `messaging`、 `microphone`、 `motion`、 `notifications`、 `phone`、 `radios`、 `tasks`、 `syncWithDevices`、 `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="7f628-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="7f628-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="7f628-144">appPackageFamilyName</span></span>|<span data-ttu-id="7f628-145">String</span><span class="sxs-lookup"><span data-stu-id="7f628-145">String</span></span>|<span data-ttu-id="7f628-146">Windows アプリケーションのパッケージ ファミリ名です。</span><span class="sxs-lookup"><span data-stu-id="7f628-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="7f628-147">アクセス レベルを設定すると、指定したアプリケーションを適用します。</span><span class="sxs-lookup"><span data-stu-id="7f628-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="7f628-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="7f628-148">appDisplayName</span></span>|<span data-ttu-id="7f628-149">String</span><span class="sxs-lookup"><span data-stu-id="7f628-149">String</span></span>|<span data-ttu-id="7f628-150">Windows アプリケーションのパッケージ ファミリ名です。</span><span class="sxs-lookup"><span data-stu-id="7f628-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="7f628-151">アクセス レベルを設定すると、指定したアプリケーションを適用します。</span><span class="sxs-lookup"><span data-stu-id="7f628-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="7f628-152">応答</span><span class="sxs-lookup"><span data-stu-id="7f628-152">Response</span></span>
<span data-ttu-id="7f628-153">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7f628-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f628-154">例</span><span class="sxs-lookup"><span data-stu-id="7f628-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f628-155">要求</span><span class="sxs-lookup"><span data-stu-id="7f628-155">Request</span></span>
<span data-ttu-id="7f628-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f628-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f628-157">応答</span><span class="sxs-lookup"><span data-stu-id="7f628-157">Response</span></span>
<span data-ttu-id="7f628-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f628-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




