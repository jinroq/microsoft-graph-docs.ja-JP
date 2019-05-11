---
title: windowsFirewallRule リソースの種類
description: Windows ファイアウォールを介したトラフィックを制御するルール。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbf322718bd3b95e27583350bf840cc05f2e6ca0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944062"
---
# <a name="windowsfirewallrule-resource-type"></a>windowsFirewallRule リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows ファイアウォールを介したトラフィックを制御するルール。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ルールの表示名。 一意である必要はありません。|
|description|String|ルールの説明。|
|パッケージ Efamilyname|String|ファイアウォールルールの影響を受ける Microsoft Store アプリケーションのパッケージファミリー名。|
|パス|String|ファイアウォールルールの影響を受けるアプリの完全なファイルパス。|
|serviceName|String|アプリケーションではなく、サービスがトラフィックを送受信している場合に使用される名前。|
|プロトコール|Int32|0-255 IP プロトコルを表す番号 (TCP = 6、UDP = 17)。 指定しない場合、既定値は All です。 有効な値は 0 ~ 255|
|localPortRanges|String collection|ローカルポート範囲のリスト。 たとえば、"100-120"、"200"、"300-320" などです。 指定しない場合、既定値は All です。|
|remotePortRanges|String collection|リモートポート範囲の一覧。 たとえば、"100-120"、"200"、"300-320" などです。 指定しない場合、既定値は All です。|
|localAddressRanges|String collection|ルールでカバーされているローカルアドレスのリスト。 有効なトークンは次のとおりです。
- "*" はローカルアドレスを示します。 指定する場合は、このトークンのみが含まれている必要があります。
- サブネットは、サブネットマスクまたはネットワークプレフィックス表記のどちらかを使用して指定できます。 サブネットマスクもネットワークプレフィックスも指定されていない場合、サブネットマスクは既定で255.255.255.255 になります。
- 有効な IPv6 アドレス。
- スペースを含まない「開始アドレスと終了アドレス」の形式の IPv4 アドレス範囲。
- 「開始アドレス-終了アドレス」の形式の IPv6 アドレス範囲。スペースは含まれません。
既定は任意のアドレスです。 || remoteAddressRanges |文字列コレクション |ルールの対象となるリモートアドレスを指定するトークンの一覧です。 トークンの大文字と小文字は区別されません。 有効なトークンは次のとおりです。
- "*" は任意のリモートアドレスを示します。 指定する場合は、このトークンのみが含まれている必要があります。
- "Defaultgateway"
- DHCP
- DSN
- 獲得
- "Intranet" (Windows バージョンでサポートされている 1809 +)
- "RmtIntranet" (Windows バージョンでサポートされている 1809 +)
- "Internet" (Windows バージョンでサポートされている 1809 +)
- "Ply2Renders" (Windows バージョン1809以降でサポートされています)
- "LocalSubnet" は、ローカルサブネット上のローカルアドレスを示します。
- サブネットは、サブネットマスクまたはネットワークプレフィックス表記のどちらかを使用して指定できます。 サブネットマスクもネットワークプレフィックスも指定されていない場合、サブネットマスクは既定で255.255.255.255 になります。
- 有効な IPv6 アドレス。
- スペースを含まない「開始アドレスと終了アドレス」の形式の IPv4 アドレス範囲。
- 「開始アドレス-終了アドレス」の形式の IPv6 アドレス範囲。スペースは含まれません。
既定は任意のアドレスです。 || profileTypes |[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|ルールが属するプロファイルを指定します。 指定しない場合、既定値は All です。 可能な値: `notConfigured`、 `domain`、 `private`、 `public`。 || action |[Statemanagementsetting](../resources/intune-deviceconfig-statemanagementsetting.md)|ルールによって適用されるアクション。 指定しない場合、既定値を使用できます。 可能な値: `notConfigured`、 `blocked`、 `allowed`. || trafficDirection |[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|ルールが有効になっているトラフィックの方向。 指定しない場合、既定値は "Out" です。可能な値: `notConfigured`、 `out`、 `in`. || interfaceTypes |[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|ルールのインターフェイスの種類。 可能な値: `notConfigured`、 `remoteAccess`、 `wireless`、 `lan`。 || localUserAuthorizations |文字列 |アプリコンテナーに対して承認されたローカルユーザーのリストを指定します。 これは、セキュリティ記述子定義言語 (SDDL) 形式の文字列です。 |

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "localUserAuthorizations": "String"
}
```




