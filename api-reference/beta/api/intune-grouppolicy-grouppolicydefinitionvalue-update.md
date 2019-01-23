---
title: GroupPolicyDefinitionValue を更新します。
description: GroupPolicyDefinitionValue オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d346a40e5ee8c2cba6f1510cf52d747e85a0b788
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430260"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="6c15c-103">GroupPolicyDefinitionValue を更新します。</span><span class="sxs-lookup"><span data-stu-id="6c15c-103">Update groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="6c15c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c15c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c15c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c15c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c15c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6c15c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c15c-107">[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6c15c-107">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c15c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6c15c-108">Prerequisites</span></span>
<span data-ttu-id="6c15c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c15c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6c15c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c15c-111">Permission type</span></span>|<span data-ttu-id="6c15c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c15c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c15c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c15c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c15c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c15c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6c15c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c15c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c15c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c15c-116">Not supported.</span></span>|
|<span data-ttu-id="6c15c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c15c-117">Application</span></span>|<span data-ttu-id="6c15c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c15c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c15c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c15c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="6c15c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c15c-120">Request headers</span></span>
|<span data-ttu-id="6c15c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c15c-121">Header</span></span>|<span data-ttu-id="6c15c-122">値</span><span class="sxs-lookup"><span data-stu-id="6c15c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c15c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c15c-123">Authorization</span></span>|<span data-ttu-id="6c15c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6c15c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c15c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6c15c-125">Accept</span></span>|<span data-ttu-id="6c15c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c15c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c15c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c15c-127">Request body</span></span>
<span data-ttu-id="6c15c-128">要求の本文に[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c15c-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="6c15c-129">[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="6c15c-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="6c15c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c15c-130">Property</span></span>|<span data-ttu-id="6c15c-131">型</span><span class="sxs-lookup"><span data-stu-id="6c15c-131">Type</span></span>|<span data-ttu-id="6c15c-132">説明</span><span class="sxs-lookup"><span data-stu-id="6c15c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c15c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c15c-133">createdDateTime</span></span>|<span data-ttu-id="6c15c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c15c-134">DateTimeOffset</span></span>|<span data-ttu-id="6c15c-135">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6c15c-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="6c15c-136">enabled</span><span class="sxs-lookup"><span data-stu-id="6c15c-136">enabled</span></span>|<span data-ttu-id="6c15c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c15c-137">Boolean</span></span>|<span data-ttu-id="6c15c-138">有効または、関連付けられているグループ ポリシーの定義を無効にします。</span><span class="sxs-lookup"><span data-stu-id="6c15c-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="6c15c-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="6c15c-139">configurationType</span></span>|[<span data-ttu-id="6c15c-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="6c15c-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="6c15c-141">値を構成する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c15c-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="6c15c-142">ポリシーとして、または環境設定のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="6c15c-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="6c15c-143">使用可能な値は、`policy`、`preference` です。</span><span class="sxs-lookup"><span data-stu-id="6c15c-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="6c15c-144">id</span><span class="sxs-lookup"><span data-stu-id="6c15c-144">id</span></span>|<span data-ttu-id="6c15c-145">String</span><span class="sxs-lookup"><span data-stu-id="6c15c-145">String</span></span>|<span data-ttu-id="6c15c-146">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6c15c-146">Key of the entity.</span></span>|
|<span data-ttu-id="6c15c-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c15c-147">lastModifiedDateTime</span></span>|<span data-ttu-id="6c15c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c15c-148">DateTimeOffset</span></span>|<span data-ttu-id="6c15c-149">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="6c15c-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6c15c-150">応答</span><span class="sxs-lookup"><span data-stu-id="6c15c-150">Response</span></span>
<span data-ttu-id="6c15c-151">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6c15c-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c15c-152">例</span><span class="sxs-lookup"><span data-stu-id="6c15c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c15c-153">要求</span><span class="sxs-lookup"><span data-stu-id="6c15c-153">Request</span></span>
<span data-ttu-id="6c15c-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c15c-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="6c15c-155">応答</span><span class="sxs-lookup"><span data-stu-id="6c15c-155">Response</span></span>
<span data-ttu-id="6c15c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6c15c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




