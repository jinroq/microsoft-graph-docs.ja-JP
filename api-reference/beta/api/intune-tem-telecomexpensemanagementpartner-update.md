---
title: telecomExpenseManagementPartner の更新
description: telecomExpenseManagementPartner オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b13c382e773b7e67fe751520d73cb8ded6b2196
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979541"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="aa494-103">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="aa494-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="aa494-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa494-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa494-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa494-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa494-106">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa494-106">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa494-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="aa494-107">Prerequisites</span></span>
<span data-ttu-id="aa494-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aa494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa494-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aa494-110">Permission type</span></span>|<span data-ttu-id="aa494-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aa494-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa494-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aa494-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa494-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa494-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aa494-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aa494-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa494-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa494-115">Not supported.</span></span>|
|<span data-ttu-id="aa494-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aa494-116">Application</span></span>|<span data-ttu-id="aa494-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa494-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa494-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aa494-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="aa494-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa494-119">Request headers</span></span>
|<span data-ttu-id="aa494-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa494-120">Header</span></span>|<span data-ttu-id="aa494-121">値</span><span class="sxs-lookup"><span data-stu-id="aa494-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa494-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa494-122">Authorization</span></span>|<span data-ttu-id="aa494-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa494-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa494-124">承諾</span><span class="sxs-lookup"><span data-stu-id="aa494-124">Accept</span></span>|<span data-ttu-id="aa494-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa494-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa494-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="aa494-126">Request body</span></span>
<span data-ttu-id="aa494-127">要求本文で、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="aa494-127">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="aa494-128">次の表に、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="aa494-128">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="aa494-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa494-129">Property</span></span>|<span data-ttu-id="aa494-130">型</span><span class="sxs-lookup"><span data-stu-id="aa494-130">Type</span></span>|<span data-ttu-id="aa494-131">説明</span><span class="sxs-lookup"><span data-stu-id="aa494-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa494-132">id</span><span class="sxs-lookup"><span data-stu-id="aa494-132">id</span></span>|<span data-ttu-id="aa494-133">文字列</span><span class="sxs-lookup"><span data-stu-id="aa494-133">String</span></span>|<span data-ttu-id="aa494-134">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="aa494-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="aa494-135">displayName</span><span class="sxs-lookup"><span data-stu-id="aa494-135">displayName</span></span>|<span data-ttu-id="aa494-136">String</span><span class="sxs-lookup"><span data-stu-id="aa494-136">String</span></span>|<span data-ttu-id="aa494-137">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="aa494-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="aa494-138">url</span><span class="sxs-lookup"><span data-stu-id="aa494-138">url</span></span>|<span data-ttu-id="aa494-139">String</span><span class="sxs-lookup"><span data-stu-id="aa494-139">String</span></span>|<span data-ttu-id="aa494-140">TEM パートナーの管理用コントロール パネルの URL。管理者は、このパネルで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="aa494-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="aa494-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="aa494-141">appAuthorized</span></span>|<span data-ttu-id="aa494-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa494-142">Boolean</span></span>|<span data-ttu-id="aa494-143">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aa494-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="aa494-144">enabled</span><span class="sxs-lookup"><span data-stu-id="aa494-144">enabled</span></span>|<span data-ttu-id="aa494-145">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="aa494-145">Boolean</span></span>|<span data-ttu-id="aa494-146">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを示します。</span><span class="sxs-lookup"><span data-stu-id="aa494-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="aa494-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="aa494-147">lastConnectionDateTime</span></span>|<span data-ttu-id="aa494-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa494-148">DateTimeOffset</span></span>|<span data-ttu-id="aa494-149">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="aa494-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="aa494-150">応答</span><span class="sxs-lookup"><span data-stu-id="aa494-150">Response</span></span>
<span data-ttu-id="aa494-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aa494-151">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa494-152">例</span><span class="sxs-lookup"><span data-stu-id="aa494-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa494-153">要求</span><span class="sxs-lookup"><span data-stu-id="aa494-153">Request</span></span>
<span data-ttu-id="aa494-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aa494-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="aa494-155">応答</span><span class="sxs-lookup"><span data-stu-id="aa494-155">Response</span></span>
<span data-ttu-id="aa494-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa494-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```





