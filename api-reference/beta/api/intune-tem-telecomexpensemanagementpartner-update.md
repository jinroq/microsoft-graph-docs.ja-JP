---
title: telecomExpenseManagementPartner の更新
description: telecomExpenseManagementPartner オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 66aa8e5bb4364de37319d0c3df8c359ff259fe7a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403463"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="bc03b-103">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="bc03b-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="bc03b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc03b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc03b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc03b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc03b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc03b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc03b-107">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc03b-107">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc03b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bc03b-108">Prerequisites</span></span>
<span data-ttu-id="bc03b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc03b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc03b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc03b-111">Permission type</span></span>|<span data-ttu-id="bc03b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc03b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc03b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc03b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc03b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc03b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bc03b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc03b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc03b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc03b-116">Not supported.</span></span>|
|<span data-ttu-id="bc03b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc03b-117">Application</span></span>|<span data-ttu-id="bc03b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc03b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc03b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc03b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="bc03b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc03b-120">Request headers</span></span>
|<span data-ttu-id="bc03b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc03b-121">Header</span></span>|<span data-ttu-id="bc03b-122">値</span><span class="sxs-lookup"><span data-stu-id="bc03b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc03b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc03b-123">Authorization</span></span>|<span data-ttu-id="bc03b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bc03b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc03b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc03b-125">Accept</span></span>|<span data-ttu-id="bc03b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc03b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc03b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc03b-127">Request body</span></span>
<span data-ttu-id="bc03b-128">要求本文で、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bc03b-128">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="bc03b-129">次の表に、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bc03b-129">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="bc03b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc03b-130">Property</span></span>|<span data-ttu-id="bc03b-131">型</span><span class="sxs-lookup"><span data-stu-id="bc03b-131">Type</span></span>|<span data-ttu-id="bc03b-132">説明</span><span class="sxs-lookup"><span data-stu-id="bc03b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc03b-133">id</span><span class="sxs-lookup"><span data-stu-id="bc03b-133">id</span></span>|<span data-ttu-id="bc03b-134">String</span><span class="sxs-lookup"><span data-stu-id="bc03b-134">String</span></span>|<span data-ttu-id="bc03b-135">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="bc03b-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="bc03b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bc03b-136">displayName</span></span>|<span data-ttu-id="bc03b-137">String</span><span class="sxs-lookup"><span data-stu-id="bc03b-137">String</span></span>|<span data-ttu-id="bc03b-138">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="bc03b-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="bc03b-139">url</span><span class="sxs-lookup"><span data-stu-id="bc03b-139">url</span></span>|<span data-ttu-id="bc03b-140">String</span><span class="sxs-lookup"><span data-stu-id="bc03b-140">String</span></span>|<span data-ttu-id="bc03b-141">TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="bc03b-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="bc03b-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="bc03b-142">appAuthorized</span></span>|<span data-ttu-id="bc03b-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc03b-143">Boolean</span></span>|<span data-ttu-id="bc03b-144">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bc03b-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="bc03b-145">enabled</span><span class="sxs-lookup"><span data-stu-id="bc03b-145">enabled</span></span>|<span data-ttu-id="bc03b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc03b-146">Boolean</span></span>|<span data-ttu-id="bc03b-147">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bc03b-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="bc03b-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="bc03b-148">lastConnectionDateTime</span></span>|<span data-ttu-id="bc03b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc03b-149">DateTimeOffset</span></span>|<span data-ttu-id="bc03b-150">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="bc03b-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="bc03b-151">応答</span><span class="sxs-lookup"><span data-stu-id="bc03b-151">Response</span></span>
<span data-ttu-id="bc03b-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bc03b-152">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc03b-153">例</span><span class="sxs-lookup"><span data-stu-id="bc03b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc03b-154">要求</span><span class="sxs-lookup"><span data-stu-id="bc03b-154">Request</span></span>
<span data-ttu-id="bc03b-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bc03b-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc03b-156">応答</span><span class="sxs-lookup"><span data-stu-id="bc03b-156">Response</span></span>
<span data-ttu-id="bc03b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bc03b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




