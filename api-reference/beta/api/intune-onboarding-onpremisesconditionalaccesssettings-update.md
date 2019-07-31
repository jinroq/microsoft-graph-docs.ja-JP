---
title: onPremisesConditionalAccessSettings の更新
description: onPremisesConditionalAccessSettings オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af5b818aa57d0604b4a4fdedaf318815d0c8a020
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994013"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="a84a0-103">onPremisesConditionalAccessSettings の更新</span><span class="sxs-lookup"><span data-stu-id="a84a0-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="a84a0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a84a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a84a0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a84a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a84a0-106">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a84a0-106">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a84a0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a84a0-107">Prerequisites</span></span>
<span data-ttu-id="a84a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a84a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a84a0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a84a0-110">Permission type</span></span>|<span data-ttu-id="a84a0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a84a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a84a0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a84a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a84a0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a84a0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a84a0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a84a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a84a0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a84a0-115">Not supported.</span></span>|
|<span data-ttu-id="a84a0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a84a0-116">Application</span></span>|<span data-ttu-id="a84a0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a84a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a84a0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a84a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="a84a0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a84a0-119">Request headers</span></span>
|<span data-ttu-id="a84a0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a84a0-120">Header</span></span>|<span data-ttu-id="a84a0-121">値</span><span class="sxs-lookup"><span data-stu-id="a84a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a84a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a84a0-122">Authorization</span></span>|<span data-ttu-id="a84a0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a84a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a84a0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a84a0-124">Accept</span></span>|<span data-ttu-id="a84a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a84a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a84a0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a84a0-126">Request body</span></span>
<span data-ttu-id="a84a0-127">要求本文で、[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a84a0-127">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="a84a0-128">次の表に、[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a84a0-128">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="a84a0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a84a0-129">Property</span></span>|<span data-ttu-id="a84a0-130">型</span><span class="sxs-lookup"><span data-stu-id="a84a0-130">Type</span></span>|<span data-ttu-id="a84a0-131">説明</span><span class="sxs-lookup"><span data-stu-id="a84a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a84a0-132">id</span><span class="sxs-lookup"><span data-stu-id="a84a0-132">id</span></span>|<span data-ttu-id="a84a0-133">String</span><span class="sxs-lookup"><span data-stu-id="a84a0-133">String</span></span>|<span data-ttu-id="a84a0-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a84a0-134">Not yet documented</span></span>|
|<span data-ttu-id="a84a0-135">enabled</span><span class="sxs-lookup"><span data-stu-id="a84a0-135">enabled</span></span>|<span data-ttu-id="a84a0-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="a84a0-136">Boolean</span></span>|<span data-ttu-id="a84a0-137">対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a84a0-137">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="a84a0-138">includedGroups</span><span class="sxs-lookup"><span data-stu-id="a84a0-138">includedGroups</span></span>|<span data-ttu-id="a84a0-139">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="a84a0-139">Guid collection</span></span>|<span data-ttu-id="a84a0-140">オンプレミスの条件付きアクセスで対象となるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="a84a0-140">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="a84a0-141">これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="a84a0-141">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="a84a0-142">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="a84a0-142">excludedGroups</span></span>|<span data-ttu-id="a84a0-143">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="a84a0-143">Guid collection</span></span>|<span data-ttu-id="a84a0-144">オンプレミスの条件付きアクセスで除外されるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="a84a0-144">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="a84a0-145">これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。</span><span class="sxs-lookup"><span data-stu-id="a84a0-145">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="a84a0-146">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="a84a0-146">overrideDefaultRule</span></span>|<span data-ttu-id="a84a0-147">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="a84a0-147">Boolean</span></span>|<span data-ttu-id="a84a0-148">デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="a84a0-148">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="a84a0-149">応答</span><span class="sxs-lookup"><span data-stu-id="a84a0-149">Response</span></span>
<span data-ttu-id="a84a0-150">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a84a0-150">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a84a0-151">例</span><span class="sxs-lookup"><span data-stu-id="a84a0-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="a84a0-152">要求</span><span class="sxs-lookup"><span data-stu-id="a84a0-152">Request</span></span>
<span data-ttu-id="a84a0-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a84a0-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="a84a0-154">応答</span><span class="sxs-lookup"><span data-stu-id="a84a0-154">Response</span></span>
<span data-ttu-id="a84a0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a84a0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```





