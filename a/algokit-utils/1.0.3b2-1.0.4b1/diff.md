# Comparing `tmp/algokit_utils-1.0.3b2-py3-none-any.whl.zip` & `tmp/algokit_utils-1.0.4b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 30666 bytes, number of entries: 14
--rw-r--r--  2.0 unx     3476 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
--rw-r--r--  2.0 unx     3513 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
--rw-r--r--  2.0 unx     7508 b- defN 80-Jan-01 00:00 algokit_utils/account.py
--rw-r--r--  2.0 unx    65567 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
--rw-r--r--  2.0 unx     7424 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
--rw-r--r--  2.0 unx    19351 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
--rw-r--r--  2.0 unx     1931 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
--rw-r--r--  2.0 unx      934 b- defN 80-Jan-01 00:00 algokit_utils/models.py
--rw-r--r--  2.0 unx     3824 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
+Zip file size: 31268 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     3493 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
+-rw-r--r--  2.0 unx     3568 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
+-rw-r--r--  2.0 unx     7709 b- defN 80-Jan-01 00:00 algokit_utils/account.py
+-rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
+-rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
+-rw-r--r--  2.0 unx    29956 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
+-rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
+-rw-r--r--  2.0 unx     3930 b- defN 80-Jan-01 00:00 algokit_utils/models.py
+-rw-r--r--  2.0 unx     3838 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1873 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.3b2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1174 b- defN 16-Jan-01 00:00 algokit_utils-1.0.3b2.dist-info/RECORD
-14 files, 117739 bytes uncompressed, 28712 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1873 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.0.4b1.dist-info/RECORD
+14 files, 120059 bytes uncompressed, 29314 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.0.3b2.dist-info/LICENSE
+Filename: algokit_utils-1.0.4b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.0.3b2.dist-info/METADATA
+Filename: algokit_utils-1.0.4b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.0.3b2.dist-info/WHEEL
+Filename: algokit_utils-1.0.4b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.0.3b2.dist-info/RECORD
+Filename: algokit_utils-1.0.4b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/__init__.py

```diff
@@ -9,30 +9,17 @@
     get_dispenser_account,
     get_kmd_wallet_account,
     get_localnet_default_account,
     get_or_create_kmd_wallet_account,
     get_sandbox_default_account,
 )
 from algokit_utils.application_client import (
-    ABIArgsDict,
-    ABICallArgs,
-    ABICallArgsDict,
-    ABICreateCallArgs,
-    ABICreateCallArgsDict,
-    ABIMethod,
     ApplicationClient,
-    CommonCallParameters,
-    CommonCallParametersDict,
-    CreateCallParameters,
-    CreateCallParametersDict,
-    OnCompleteCallParameters,
-    OnCompleteCallParametersDict,
     Program,
     execute_atc_with_logic_error,
-    get_app_id_from_tx_id,
     get_next_version,
     get_sender_from_signer,
     num_extra_program_pages,
 )
 from algokit_utils.application_specification import (
     ApplicationSpecification,
     AppSpecStateDict,
@@ -43,30 +30,47 @@
     MethodHints,
     OnCompleteActionName,
 )
 from algokit_utils.deploy import (
     DELETABLE_TEMPLATE_NAME,
     NOTE_PREFIX,
     UPDATABLE_TEMPLATE_NAME,
+    ABICallArgs,
+    ABICallArgsDict,
+    ABICreateCallArgs,
+    ABICreateCallArgsDict,
     AppDeployMetaData,
     AppLookup,
     AppMetaData,
     AppReference,
     DeploymentFailedError,
     DeployResponse,
     OnSchemaBreak,
     OnUpdate,
     OperationPerformed,
     TemplateValueDict,
     TemplateValueMapping,
+    get_app_id_from_tx_id,
     get_creator_apps,
     replace_template_variables,
 )
 from algokit_utils.logic_error import LogicError
-from algokit_utils.models import ABITransactionResponse, Account, TransactionResponse
+from algokit_utils.models import (
+    ABIArgsDict,
+    ABIMethod,
+    ABITransactionResponse,
+    Account,
+    CommonCallParameters,
+    CommonCallParametersDict,
+    CreateCallParameters,
+    CreateCallParametersDict,
+    OnCompleteCallParameters,
+    OnCompleteCallParametersDict,
+    TransactionResponse,
+)
 from algokit_utils.network_clients import (
     AlgoClientConfig,
     get_algod_client,
     get_indexer_client,
     get_kmd_client_from_algod_client,
     is_localnet,
     is_sandbox,
```

## algokit_utils/_transfer.py

```diff
@@ -1,18 +1,21 @@
 import dataclasses
 import logging
+from typing import TYPE_CHECKING
 
 import algosdk.transaction
 from algosdk.account import address_from_private_key
 from algosdk.atomic_transaction_composer import AccountTransactionSigner
 from algosdk.transaction import PaymentTxn, SuggestedParams
-from algosdk.v2client.algod import AlgodClient
 
 from algokit_utils.models import Account
 
+if TYPE_CHECKING:
+    from algosdk.v2client.algod import AlgodClient
+
 __all__ = ["TransferParameters", "transfer"]
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass(kw_only=True)
 class TransferParameters:
     """Parameters for transferring µALGOs between accounts"""
@@ -26,36 +29,36 @@
     suggested_params: SuggestedParams | None = None
     """(optional) transaction parameters"""
     note: str | bytes | None = None
     """(optional) transaction note"""
     fee_micro_algos: int | None = None
     """(optional) The flat fee you want to pay, useful for covering extra fees in a transaction group or app call"""
     max_fee_micro_algos: int | None = None
-    """(optional)The maximum fee that you are happy to pay (default: unbounded) - 
+    """(optional)The maximum fee that you are happy to pay (default: unbounded) -
     if this is set it's possible the transaction could get rejected during network congestion"""
 
 
 def _check_fee(transaction: PaymentTxn, max_fee: int | None) -> None:
     if max_fee is not None:
         # Once a transaction has been constructed by algosdk, transaction.fee indicates what the total transaction fee
         # Will be based on the current suggested fee-per-byte value.
         if transaction.fee > max_fee:
             raise Exception(
                 f"Cancelled transaction due to high network congestion fees. "
                 f"Algorand suggested fees would cause this transaction to cost {transaction.fee} µALGOs. "
                 f"Cap for this transaction is {max_fee} µALGOs."
             )
-        elif transaction.fee > algosdk.constants.MIN_TXN_FEE:
+        if transaction.fee > algosdk.constants.MIN_TXN_FEE:
             logger.warning(
                 f"Algorand network congestion fees are in effect. "
                 f"This transaction will incur a fee of {transaction.fee} µALGOs."
             )
 
 
-def transfer(client: AlgodClient, parameters: TransferParameters) -> PaymentTxn:
+def transfer(client: "AlgodClient", parameters: TransferParameters) -> PaymentTxn:
     """Transfer µALGOs between accounts"""
 
     suggested_params = parameters.suggested_params or client.suggested_params()
     from_account = parameters.from_account
     sender = address_from_private_key(from_account.private_key)  # type: ignore[no-untyped-call]
     transaction = PaymentTxn(
         sender=sender,
```

## algokit_utils/account.py

```diff
@@ -1,59 +1,63 @@
 import logging
 import os
 import warnings
-from collections.abc import Callable
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from algosdk.account import address_from_private_key
-from algosdk.kmd import KMDClient
 from algosdk.mnemonic import from_private_key, to_private_key
 from algosdk.util import algos_to_microalgos
-from algosdk.v2client.algod import AlgodClient
 
 from algokit_utils._transfer import TransferParameters, transfer
 from algokit_utils.models import Account
 from algokit_utils.network_clients import get_kmd_client_from_algod_client, is_localnet
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
+    from algosdk.kmd import KMDClient
+    from algosdk.v2client.algod import AlgodClient
+
 __all__ = [
     "create_kmd_wallet_account",
     "get_account",
     "get_account_from_mnemonic",
     "get_dispenser_account",
     "get_kmd_wallet_account",
     "get_localnet_default_account",
     "get_or_create_kmd_wallet_account",
     "get_sandbox_default_account",
 ]
 
 logger = logging.getLogger(__name__)
+_DEFAULT_ACCOUNT_MINIMUM_BALANCE = 1_000_000_000
 
 
 def get_account_from_mnemonic(mnemonic: str) -> Account:
     """Convert a mnemonic (25 word passphrase) into an Account"""
     private_key = to_private_key(mnemonic)  # type: ignore[no-untyped-call]
     address = address_from_private_key(private_key)  # type: ignore[no-untyped-call]
-    return Account(private_key, address)
+    return Account(private_key=private_key, address=address)
 
 
-def create_kmd_wallet_account(kmd_client: KMDClient, name: str) -> Account:
+def create_kmd_wallet_account(kmd_client: "KMDClient", name: str) -> Account:
     """Creates a wallet with specified name"""
     wallet_id = kmd_client.create_wallet(name, "")["id"]  # type: ignore[no-untyped-call]
     wallet_handle = kmd_client.init_wallet_handle(wallet_id, "")  # type: ignore[no-untyped-call]
     kmd_client.generate_key(wallet_handle)  # type: ignore[no-untyped-call]
 
     key_ids: list[str] = kmd_client.list_keys(wallet_handle)  # type: ignore[no-untyped-call]
     account_key = key_ids[0]
 
     private_account_key = kmd_client.export_key(wallet_handle, "", account_key)  # type: ignore[no-untyped-call]
     return get_account_from_mnemonic(from_private_key(private_account_key))  # type: ignore[no-untyped-call]
 
 
 def get_or_create_kmd_wallet_account(
-    client: AlgodClient, name: str, fund_with_algos: float = 1000, kmd_client: KMDClient | None = None
+    client: "AlgodClient", name: str, fund_with_algos: float = 1000, kmd_client: "KMDClient | None" = None
 ) -> Account:
     """Returns a wallet with specified name, or creates one if not found"""
     kmd_client = kmd_client or get_kmd_client_from_algod_client(client)
     account = get_kmd_wallet_account(client, kmd_client, name)
 
     if account:
         account_info = client.account_info(account.address)
@@ -81,45 +85,50 @@
             ),
         )
 
     return account
 
 
 def _is_default_account(account: dict[str, Any]) -> bool:
-    return bool(account["status"] != "Offline" and account["amount"] > 1_000_000_000)
+    return bool(account["status"] != "Offline" and account["amount"] > _DEFAULT_ACCOUNT_MINIMUM_BALANCE)
 
 
-def get_sandbox_default_account(client: AlgodClient) -> Account:
+def get_sandbox_default_account(client: "AlgodClient") -> Account:
     warnings.warn(
-        "get_sandbox_default_account is deprecated, please use get_localnet_default_account instead", DeprecationWarning
+        "get_sandbox_default_account is deprecated, please use get_localnet_default_account instead",
+        DeprecationWarning,
+        stacklevel=2,
     )
     return get_localnet_default_account(client)
 
 
-def get_localnet_default_account(client: AlgodClient) -> Account:
+def get_localnet_default_account(client: "AlgodClient") -> Account:
     """Returns the default Account in a LocalNet instance"""
     if not is_localnet(client):
         raise Exception("Can't get a default account from non LocalNet network")
 
     account = get_kmd_wallet_account(
         client, get_kmd_client_from_algod_client(client), "unencrypted-default-wallet", _is_default_account
     )
     assert account
     return account
 
 
-def get_dispenser_account(client: AlgodClient) -> Account:
+def get_dispenser_account(client: "AlgodClient") -> Account:
     """Returns an Account based on DISPENSER_MNENOMIC environment variable or the default account on LocalNet"""
     if is_localnet(client):
         return get_localnet_default_account(client)
     return get_account(client, "DISPENSER")
 
 
 def get_kmd_wallet_account(
-    client: AlgodClient, kmd_client: KMDClient, name: str, predicate: Callable[[dict[str, Any]], bool] | None = None
+    client: "AlgodClient",
+    kmd_client: "KMDClient",
+    name: str,
+    predicate: "Callable[[dict[str, Any]], bool] | None" = None,
 ) -> Account | None:
     """Returns wallet matching specified name and predicate or None if not found"""
     wallets: list[dict] = kmd_client.list_wallets()  # type: ignore[no-untyped-call]
 
     wallet = next((w for w in wallets if w["name"] == name), None)
     if wallet is None:
         return None
@@ -141,15 +150,15 @@
         return None
 
     private_account_key = kmd_client.export_key(wallet_handle, "", matched_account_key)  # type: ignore[no-untyped-call]
     return get_account_from_mnemonic(from_private_key(private_account_key))  # type: ignore[no-untyped-call]
 
 
 def get_account(
-    client: AlgodClient, name: str, fund_with_algos: float = 1000, kmd_client: KMDClient | None = None
+    client: "AlgodClient", name: str, fund_with_algos: float = 1000, kmd_client: "KMDClient | None" = None
 ) -> Account:
     """Returns an Algorand account with private key loaded by convention based on the given name identifier.
 
     # Convention
 
     **Non-LocalNet:** will load `os.environ[f"{name}_MNEMONIC"]` as a mnemonic secret
     Be careful how the mnemonic is handled, never commit it into source control and ideally load it via a
```

## algokit_utils/application_client.py

```diff
@@ -1,17 +1,15 @@
 import base64
 import copy
-import dataclasses
 import logging
 import re
 import typing
-from collections.abc import Sequence
 from math import ceil
 from pathlib import Path
-from typing import Any, Literal, TypedDict, cast, overload
+from typing import Any, Literal, cast, overload
 
 import algosdk
 from algosdk import transaction
 from algosdk.abi import ABIType, Method, Returns
 from algosdk.account import address_from_private_key
 from algosdk.atomic_transaction_composer import (
     ABI_RETURN_HASH,
@@ -23,66 +21,59 @@
     MultisigTransactionSigner,
     TransactionSigner,
     TransactionWithSigner,
 )
 from algosdk.constants import APP_PAGE_MAX_SIZE
 from algosdk.logic import get_application_address
 from algosdk.source_map import SourceMap
-from algosdk.v2client.algod import AlgodClient
-from algosdk.v2client.indexer import IndexerClient
 
 import algokit_utils.application_specification as au_spec
 import algokit_utils.deploy as au_deploy
-from algokit_utils.deploy import check_app_and_deploy
 from algokit_utils.logic_error import LogicError, parse_logic_error
-from algokit_utils.models import ABITransactionResponse, Account, TransactionResponse
+from algokit_utils.models import (
+    ABIArgsDict,
+    ABIArgType,
+    ABIMethod,
+    ABITransactionResponse,
+    Account,
+    CommonCallParameters,
+    CommonCallParametersDict,
+    CreateCallParameters,
+    CreateCallParametersDict,
+    OnCompleteCallParameters,
+    OnCompleteCallParametersDict,
+    TransactionResponse,
+)
+
+if typing.TYPE_CHECKING:
+    from algosdk.v2client.algod import AlgodClient
+    from algosdk.v2client.indexer import IndexerClient
+
 
 logger = logging.getLogger(__name__)
 
-ABIArgType = Any
-ABIArgsDict = dict[str, ABIArgType]
 """A dictionary `dict[str, Any]` representing ABI argument names and values"""
 
 __all__ = [
-    "ABIArgsDict",
-    "ABICallArgs",
-    "ABICallArgsDict",
-    "ABICreateCallArgs",
-    "ABICreateCallArgsDict",
-    "ABIMethod",
     "ApplicationClient",
-    "CommonCallParameters",
-    "CommonCallParametersDict",
-    "OnCompleteCallParameters",
-    "OnCompleteCallParametersDict",
-    "CreateCallParameters",
-    "CreateCallParametersDict",
     "Program",
     "execute_atc_with_logic_error",
-    "get_app_id_from_tx_id",
     "get_next_version",
     "get_sender_from_signer",
     "num_extra_program_pages",
 ]
 
-
-class ABIReturnSubroutine(typing.Protocol):
-    def method_spec(self) -> Method:
-        ...
-
-
-ABIMethod: typing.TypeAlias = ABIReturnSubroutine | Method | str
-"""Alias for {py:class}`pyteal.ABIReturnSubroutine`, {py:class}`algosdk.abi.method.Method` or a {py:class}`str` 
+"""Alias for {py:class}`pyteal.ABIReturnSubroutine`, {py:class}`algosdk.abi.method.Method` or a {py:class}`str`
 representing an ABI method name or signature"""
 
 
 class Program:
     """A compiled TEAL program"""
 
-    def __init__(self, program: str, client: AlgodClient):
+    def __init__(self, program: str, client: "AlgodClient"):
         """
         Fully compile the program source to binary and generate a
         source map for matching pc to line number
         """
         self.teal = program
         result: dict = client.compile(au_deploy.strip_comments(self.teal), source_map=True)
         self.raw_binary = base64.b64decode(result["result"])
@@ -92,153 +83,55 @@
 
 def num_extra_program_pages(approval: bytes, clear: bytes) -> int:
     """Calculate minimum number of extra_pages required for provided approval and clear programs"""
 
     return ceil(((len(approval) + len(clear)) - APP_PAGE_MAX_SIZE) / APP_PAGE_MAX_SIZE)
 
 
-@dataclasses.dataclass(kw_only=True)
-class CommonCallParameters:
-    """Common transaction parameters used when making update, delete, opt_in, close_out or clear_state calls"""
-
-    signer: TransactionSigner | None = None
-    sender: str | None = None
-    suggested_params: transaction.SuggestedParams | None = None
-    note: bytes | str | None = None
-    lease: bytes | str | None = None
-    accounts: list[str] | None = None
-    foreign_apps: list[int] | None = None
-    foreign_assets: list[int] | None = None
-    boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
-    rekey_to: str | None = None
-
-
-@dataclasses.dataclass(kw_only=True)
-class OnCompleteCallParameters(CommonCallParameters):
-    """Transaction parameters used when making any call to an Application"""
-
-    on_complete: transaction.OnComplete | None = None
-
-
-@dataclasses.dataclass(kw_only=True)
-class CreateCallParameters(OnCompleteCallParameters):
-    """Transaction parameters used when making a create call for Application"""
-
-    extra_pages: int | None = None
-
-
-class CommonCallParametersDict(TypedDict, total=False):
-    """Common transaction parameters used when making update, delete, opt_in, close_out or clear_state calls"""
-
-    signer: TransactionSigner
-    sender: str
-    suggested_params: transaction.SuggestedParams
-    note: bytes | str
-    lease: bytes | str
-
-
-class OnCompleteCallParametersDict(TypedDict, CommonCallParametersDict, total=False):
-    """Transaction parameters used when making any call to an Application"""
-
-    on_complete: transaction.OnComplete
-
-
-class CreateCallParametersDict(TypedDict, OnCompleteCallParametersDict, total=False):
-    """Transaction parameters used when making a create call for Application"""
-
-    extra_pages: int
-
-
-@dataclasses.dataclass(kw_only=True)
-class ABICallArgs:
-    """Parameters used to update or delete an application when calling
-    {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
-
-    method: ABIMethod | bool | None = None
-    args: ABIArgsDict = dataclasses.field(default_factory=dict)
-    suggested_params: transaction.SuggestedParams | None = None
-    lease: bytes | str | None = None
-    accounts: list[str] | None = None
-    foreign_apps: list[int] | None = None
-    foreign_assets: list[int] | None = None
-    boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
-    rekey_to: str | None = None
-
-
-@dataclasses.dataclass(kw_only=True)
-class ABICreateCallArgs(ABICallArgs):
-    """Parameters used to create an application when calling {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
-
-    extra_pages: int | None = None
-    on_complete: transaction.OnComplete | None = None
-
-
-class ABICallArgsDict(TypedDict, total=False):
-    """Parameters used to update or delete an application when calling
-    {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
-
-    method: ABIMethod | bool
-    args: ABIArgsDict
-    suggested_params: transaction.SuggestedParams
-    lease: bytes | str
-    accounts: list[str]
-    foreign_apps: list[int]
-    foreign_assets: list[int]
-    boxes: Sequence[tuple[int, bytes | bytearray | str | int]]
-    rekey_to: str
-
-
-class ABICreateCallArgsDict(TypedDict, ABICallArgsDict, total=False):
-    """Parameters used to create an application when calling {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
-
-    extra_pages: int | None
-    on_complete: transaction.OnComplete
-
-
 class ApplicationClient:
     """A class that wraps an ARC-0032 app spec and provides high productivity methods to deploy and call the app"""
 
     @overload
     def __init__(
         self,
-        algod_client: AlgodClient,
+        algod_client: "AlgodClient",
         app_spec: au_spec.ApplicationSpecification | Path,
         *,
         app_id: int = 0,
         signer: TransactionSigner | Account | None = None,
         sender: str | None = None,
         suggested_params: transaction.SuggestedParams | None = None,
         template_values: au_deploy.TemplateValueMapping | None = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
-        algod_client: AlgodClient,
+        algod_client: "AlgodClient",
         app_spec: au_spec.ApplicationSpecification | Path,
         *,
         creator: str | Account,
-        indexer_client: IndexerClient | None = None,
+        indexer_client: "IndexerClient | None" = None,
         existing_deployments: au_deploy.AppLookup | None = None,
         signer: TransactionSigner | Account | None = None,
         sender: str | None = None,
         suggested_params: transaction.SuggestedParams | None = None,
         template_values: au_deploy.TemplateValueMapping | None = None,
     ):
         ...
 
     def __init__(
         self,
-        algod_client: AlgodClient,
+        algod_client: "AlgodClient",
         app_spec: au_spec.ApplicationSpecification | Path,
         *,
         app_id: int = 0,
         creator: str | Account | None = None,
-        indexer_client: IndexerClient | None = None,
+        indexer_client: "IndexerClient | None" = None,
         existing_deployments: au_deploy.AppLookup | None = None,
         signer: TransactionSigner | Account | None = None,
         sender: str | None = None,
         suggested_params: transaction.SuggestedParams | None = None,
         template_values: au_deploy.TemplateValueMapping | None = None,
     ):
         """ApplicationClient can be created with an app_id to interact with an existing application, alternatively
@@ -327,49 +220,52 @@
         signer: TransactionSigner | Account | None = None,
         sender: str | None = None,
         app_id: int | None = None,
         template_values: au_deploy.TemplateValueDict | None = None,
     ) -> "ApplicationClient":
         """Creates a copy of this ApplicationClient, using the new signer, sender and app_id values if provided.
         Will also substitute provided template_values into the associated app_spec in the copy"""
-        new_client = copy.copy(self)
-        new_client._prepare(new_client, signer=signer, sender=sender, app_id=app_id, template_values=template_values)
+        new_client: "ApplicationClient" = copy.copy(self)
+        new_client._prepare(  # noqa: SLF001
+            new_client, signer=signer, sender=sender, app_id=app_id, template_values=template_values
+        )
         return new_client
 
     def _prepare(
         self,
         target: "ApplicationClient",
+        *,
         signer: TransactionSigner | Account | None = None,
         sender: str | None = None,
         app_id: int | None = None,
         template_values: au_deploy.TemplateValueDict | None = None,
     ) -> None:
         target.app_id = self.app_id if app_id is None else app_id
         target.signer, target.sender = target.get_signer_sender(
             AccountTransactionSigner(signer.private_key) if isinstance(signer, Account) else signer, sender
         )
         if template_values:
-            target._approval_program, target._clear_program = substitute_template_and_compile(
+            target._approval_program, target._clear_program = substitute_template_and_compile(  # noqa: SLF001
                 target.algod_client, target.app_spec, template_values
             )
 
     def deploy(
         self,
         version: str | None = None,
         *,
         signer: TransactionSigner | None = None,
         sender: str | None = None,
         allow_update: bool | None = None,
         allow_delete: bool | None = None,
         on_update: au_deploy.OnUpdate = au_deploy.OnUpdate.Fail,
         on_schema_break: au_deploy.OnSchemaBreak = au_deploy.OnSchemaBreak.Fail,
         template_values: au_deploy.TemplateValueMapping | None = None,
-        create_args: ABICreateCallArgs | ABICreateCallArgsDict | None = None,
-        update_args: ABICallArgs | ABICallArgsDict | None = None,
-        delete_args: ABICallArgs | ABICallArgsDict | None = None,
+        create_args: au_deploy.ABICreateCallArgs | au_deploy.ABICreateCallArgsDict | None = None,
+        update_args: au_deploy.ABICallArgs | au_deploy.ABICallArgsDict | None = None,
+        delete_args: au_deploy.ABICallArgs | au_deploy.ABICallArgsDict | None = None,
     ) -> au_deploy.DeployResponse:
         """Deploy an application and update client to reference it.
 
         Idempotently deploy (create, update/delete if changed) an app against the given name via the given creator
         account, including deploy-time template placeholder substitutions.
         To understand the architecture decisions behind this functionality please see
         <https://github.com/algorandfoundation/algokit-cli/blob/main/docs/architecture-decisions/2023-01-12_smart-contract-deployment.md>
@@ -399,206 +295,56 @@
         should *NOT* include the TMPL_ prefix
         :param ABICreateCallArgs create_args: Arguments used when creating an application
         :param ABICallArgs | ABICallArgsDict update_args: Arguments used when updating an application
         :param ABICallArgs | ABICallArgsDict delete_args: Arguments used when deleting an application
         :return DeployResponse: details action taken and relevant transactions
         :raises DeploymentError: If the deployment failed due
         """
-        before = self._approval_program, self._clear_program, self.sender, self.signer, self.app_id
-        try:
-            return self._deploy(
-                version,
-                signer=signer,
-                sender=sender,
-                allow_update=allow_update,
-                allow_delete=allow_delete,
-                on_update=on_update,
-                on_schema_break=on_schema_break,
-                template_values=template_values,
-                create_args=create_args,
-                update_args=update_args,
-                delete_args=delete_args,
-            )
-        except Exception as ex:
-            # undo any prepare changes if there was an error
-            self._approval_program, self._clear_program, self.sender, self.signer, self.app_id = before
-            raise ex from None
-
-    def _deploy(
-        self,
-        version: str | None,
-        *,
-        signer: TransactionSigner | None,
-        sender: str | None,
-        allow_update: bool | None,
-        allow_delete: bool | None,
-        on_update: au_deploy.OnUpdate,
-        on_schema_break: au_deploy.OnSchemaBreak,
-        template_values: au_deploy.TemplateValueMapping | None,
-        create_args: ABICallArgs | ABICallArgsDict | None,
-        update_args: ABICallArgs | ABICallArgsDict | None,
-        delete_args: ABICallArgs | ABICallArgsDict | None,
-    ) -> au_deploy.DeployResponse:
-        """Ensures app associated with app client's creator is present and up to date"""
+        # check inputs
         if self.app_id:
             raise au_deploy.DeploymentFailedError(
                 f"Attempt to deploy app which already has an app index of {self.app_id}"
             )
-        signer, sender = self.resolve_signer_sender(signer, sender)
-        if not sender:
-            raise au_deploy.DeploymentFailedError("No sender provided, unable to deploy app")
+        try:
+            resolved_signer, resolved_sender = self.resolve_signer_sender(signer, sender)
+        except ValueError as ex:
+            raise au_deploy.DeploymentFailedError(f"{ex}, unable to deploy app") from None
         if not self._creator:
             raise au_deploy.DeploymentFailedError("No creator provided, unable to deploy app")
-        if self._creator != sender:
+        if self._creator != resolved_sender:
             raise au_deploy.DeploymentFailedError(
-                f"Attempt to deploy contract with a sender address {sender} that differs "
+                f"Attempt to deploy contract with a sender address {resolved_sender} that differs "
                 f"from the given creator address for this application client: {self._creator}"
             )
 
-        # make a copy
+        # make a copy and prepare variables
         template_values = dict(template_values or {})
         au_deploy.add_deploy_template_variables(template_values, allow_update=allow_update, allow_delete=allow_delete)
 
-        self._prepare(self, template_values=template_values)
-        approval_program, clear_program = self._check_is_compiled()
+        existing_app_metadata_or_reference = self._load_app_reference()
 
-        updatable = (
-            allow_update
-            if allow_update is not None
-            else au_deploy.get_deploy_control(
-                self.app_spec, au_deploy.UPDATABLE_TEMPLATE_NAME, transaction.OnComplete.UpdateApplicationOC
-            )
+        self._approval_program, self._clear_program = substitute_template_and_compile(
+            self.algod_client, self.app_spec, template_values
         )
-        deletable = (
-            allow_delete
-            if allow_delete is not None
-            else au_deploy.get_deploy_control(
-                self.app_spec, au_deploy.DELETABLE_TEMPLATE_NAME, transaction.OnComplete.DeleteApplicationOC
-            )
-        )
-
-        name = self.app_spec.contract.name
-
-        # TODO: allow resolve app id via environment variable
-        app = self._load_app_reference()
-
-        if version is None:
-            if app.app_id == 0:
-                version = "v1.0"
-            else:
-                assert isinstance(app, au_deploy.AppDeployMetaData)
-                version = get_next_version(app.version)
-        app_spec_note = au_deploy.AppDeployMetaData(name, version, updatable=updatable, deletable=deletable)
-
-        def create_app() -> au_deploy.DeployResponse:
-            assert self.existing_deployments
-
-            method, abi_args, parameters = _convert_deploy_args(create_args, app_spec_note, signer, sender)
-            create_response = self.create(
-                method,
-                parameters,
-                **abi_args,
-            )
-            logger.info(f"{name} ({version}) deployed successfully, with app id {self.app_id}.")
-            assert create_response.confirmed_round is not None
-            app_metadata = _create_metadata(app_spec_note, self.app_id, create_response.confirmed_round)
-            self.existing_deployments.apps[name] = app_metadata
-            return au_deploy.DeployResponse(
-                app=app_metadata, create_response=create_response, action_taken=au_deploy.OperationPerformed.Create
-            )
-
-        if app.app_id == 0:
-            logger.info(f"{name} not found in {self._creator} account, deploying app.")
-            return create_app()
-
-        def create_and_delete_app() -> au_deploy.DeployResponse:
-            assert isinstance(app, au_deploy.AppMetaData)
-            assert self.existing_deployments
-
-            logger.info(f"Replacing {name} ({app.version}) with {name} ({version}) in {self._creator} account.")
-            atc = AtomicTransactionComposer()
-            create_method, create_abi_args, create_parameters = _convert_deploy_args(
-                create_args, app_spec_note, signer, sender
-            )
-            self.compose_create(
-                atc,
-                create_method,
-                create_parameters,
-                **create_abi_args,
-            )
-            delete_method, delete_abi_args, delete_parameters = _convert_deploy_args(
-                delete_args, app_spec_note, signer, sender
-            )
-            self.compose_delete(
-                atc,
-                delete_method,
-                delete_parameters,
-                **delete_abi_args,
-            )
-            create_delete_response = self.execute_atc(atc)
-            create_response = _tr_from_atr(atc, create_delete_response, 0)
-            delete_response = _tr_from_atr(atc, create_delete_response, 1)
-            self._set_app_id_from_tx_id(create_response.tx_id)
-            logger.info(f"{name} ({version}) deployed successfully, with app id {self.app_id}.")
-            logger.info(f"{name} ({app.version}) with app id {app.app_id}, deleted successfully.")
-
-            app_metadata = _create_metadata(app_spec_note, self.app_id, create_delete_response.confirmed_round)
-            self.existing_deployments.apps[name] = app_metadata
-
-            return au_deploy.DeployResponse(
-                app=app_metadata,
-                create_response=create_response,
-                delete_response=delete_response,
-                action_taken=au_deploy.OperationPerformed.Replace,
-            )
-
-        def update_app() -> au_deploy.DeployResponse:
-            assert on_update == au_deploy.OnUpdate.UpdateApp
-            assert isinstance(app, au_deploy.AppMetaData)
-            assert self.existing_deployments
-            logger.info(f"Updating {name} to {version} in {self._creator} account, with app id {app.app_id}")
-            method, abi_args, parameters = _convert_deploy_args(update_args, app_spec_note, signer, sender)
-            update_response = self.update(
-                method,
-                parameters,
-                **abi_args,
-            )
-            app_metadata = _create_metadata(
-                app_spec_note,
-                self.app_id,
-                app.created_round,
-                updated_round=update_response.confirmed_round,
-                original_metadata=app.created_metadata,
-            )
-            self.existing_deployments.apps[name] = app_metadata
-            return au_deploy.DeployResponse(
-                app=app_metadata, update_response=update_response, action_taken=au_deploy.OperationPerformed.Update
-            )
-
-        assert isinstance(app, au_deploy.AppMetaData)
-        logger.debug(f"{name} found in {self._creator} account, with app id {app.app_id}, version={app.version}.")
-
-        app_changes = au_deploy.check_for_app_changes(
-            self.algod_client,
-            new_approval=approval_program.raw_binary,
-            new_clear=clear_program.raw_binary,
-            new_global_schema=self.app_spec.global_state_schema,
-            new_local_schema=self.app_spec.local_state_schema,
-            app_id=app.app_id,
-        )
-
-        return check_app_and_deploy(
-            app,
-            app_changes,
+        deployer = au_deploy.Deployer(
+            app_client=self,
+            creator=self._creator,
+            signer=resolved_signer,
+            sender=resolved_sender,
+            new_app_metadata=self._get_app_deploy_metadata(version, allow_update, allow_delete),
+            existing_app_metadata_or_reference=existing_app_metadata_or_reference,
             on_update=on_update,
             on_schema_break=on_schema_break,
-            update_app=update_app,
-            create_and_delete_app=create_and_delete_app,
+            create_args=create_args,
+            update_args=update_args,
+            delete_args=delete_args,
         )
 
+        return deployer.deploy()
+
     def compose_create(
         self,
         atc: AtomicTransactionComposer,
         /,
         call_abi_method: ABIMethod | bool | None = None,
         transaction_parameters: CreateCallParameters | CreateCallParametersDict | None = None,
         **abi_kwargs: ABIArgType,
@@ -665,15 +411,15 @@
         self.compose_create(
             atc,
             call_abi_method,
             transaction_parameters,
             **abi_kwargs,
         )
         create_result = self._execute_atc_tr(atc)
-        self._set_app_id_from_tx_id(create_result.tx_id)
+        self.app_id = au_deploy.get_app_id_from_tx_id(self.algod_client, create_result.tx_id)
         return create_result
 
     def compose_update(
         self,
         atc: AtomicTransactionComposer,
         /,
         call_abi_method: ABIMethod | bool | None = None,
@@ -1036,15 +782,15 @@
             dict[bytes | str, bytes | str | int],
             _decode_state(acct_state.get("app-local-state", {}).get("key-value", {}), raw=raw),
         )
 
     def resolve(self, to_resolve: au_spec.DefaultArgumentDict) -> int | str | bytes:
         """Resolves the default value for an ABI method, based on app_spec"""
 
-        def _data_check(value: Any) -> int | str | bytes:
+        def _data_check(value: object) -> int | str | bytes:
             if isinstance(value, int | str | bytes):
                 return value
             raise ValueError(f"Unexpected type for constant data: {value}")
 
         match to_resolve:
             case {"source": "constant", "data": data}:
                 return _data_check(data)
@@ -1062,14 +808,44 @@
                 return _data_check(response.return_value)
 
             case {"source": source}:
                 raise ValueError(f"Unrecognized default argument source: {source}")
             case _:
                 raise TypeError("Unable to interpret default argument specification")
 
+    def _get_app_deploy_metadata(
+        self, version: str | None, allow_update: bool | None, allow_delete: bool | None
+    ) -> au_deploy.AppDeployMetaData:
+        updatable = (
+            allow_update
+            if allow_update is not None
+            else au_deploy.get_deploy_control(
+                self.app_spec, au_deploy.UPDATABLE_TEMPLATE_NAME, transaction.OnComplete.UpdateApplicationOC
+            )
+        )
+        deletable = (
+            allow_delete
+            if allow_delete is not None
+            else au_deploy.get_deploy_control(
+                self.app_spec, au_deploy.DELETABLE_TEMPLATE_NAME, transaction.OnComplete.DeleteApplicationOC
+            )
+        )
+
+        app = self._load_app_reference()
+
+        if version is None:
+            if app.app_id == 0:
+                version = "v1.0"
+            else:
+                assert isinstance(app, au_deploy.AppDeployMetaData)
+                version = get_next_version(app.version)
+        return au_deploy.AppDeployMetaData(
+            self.app_spec.contract.name, version, updatable=updatable, deletable=deletable
+        )
+
     def _check_is_compiled(self) -> tuple[Program, Program]:
         if self._approval_program is None or self._clear_program is None:
             raise Exception(
                 "Compiled programs are not available, please provide template_values before creating or updating"
             )
         return self._approval_program, self._clear_program
 
@@ -1092,18 +868,19 @@
         self._check_app_id()
 
     def _load_app_reference(self) -> au_deploy.AppReference | au_deploy.AppMetaData:
         if not self.existing_deployments and self._creator:
             assert self._indexer_client
             self.existing_deployments = au_deploy.get_creator_apps(self._indexer_client, self._creator)
 
-        if self.existing_deployments and self.app_id == 0:
+        if self.existing_deployments:
             app = self.existing_deployments.apps.get(self.app_spec.contract.name)
             if app:
-                self.app_id = app.app_id
+                if self.app_id == 0:
+                    self.app_id = app.app_id
                 return app
 
         return au_deploy.AppReference(self.app_id, self.app_address)
 
     def _check_app_id(self) -> None:
         if self.app_id == 0:
             raise Exception(
@@ -1156,14 +933,15 @@
 
         return self.approval_source_map
 
     def add_method_call(
         self,
         atc: AtomicTransactionComposer,
         abi_method: ABIMethod | bool | None = None,
+        *,
         abi_args: ABIArgsDict | None = None,
         app_id: int | None = None,
         parameters: CommonCallParameters | CommonCallParametersDict | None = None,
         on_complete: transaction.OnComplete = transaction.OnComplete.NoOpOC,
         local_schema: transaction.StateSchema | None = None,
         global_schema: transaction.StateSchema | None = None,
         approval_program: bytes | None = None,
@@ -1211,64 +989,68 @@
                         lease=encoded_lease,
                         rekey_to=parameters.rekey_to,
                         app_args=app_args,
                     ),
                     signer=signer,
                 )
             )
-        else:  # resolve ABI method args
-            hints = self._method_hints(method)
+            return
+        # resolve ABI method args
+        args = self._get_abi_method_args(abi_args, method)
+        atc.add_method_call(
+            app_id,
+            method,
+            sender,
+            sp,
+            signer,
+            method_args=args,
+            on_complete=on_complete,
+            local_schema=local_schema,
+            global_schema=global_schema,
+            approval_program=approval_program,
+            clear_program=clear_program,
+            extra_pages=extra_pages or 0,
+            accounts=parameters.accounts,
+            foreign_apps=parameters.foreign_apps,
+            foreign_assets=parameters.foreign_assets,
+            boxes=encoded_boxes,
+            note=parameters.note.encode("utf-8") if isinstance(parameters.note, str) else parameters.note,
+            lease=encoded_lease,
+            rekey_to=parameters.rekey_to,
+        )
+
+    def _get_abi_method_args(self, abi_args: ABIArgsDict | None, method: Method) -> list:
+        args: list = []
+        hints = self._method_hints(method)
+        # copy args so we don't mutate original
+        abi_args = dict(abi_args or {})
+        for method_arg in method.args:
+            name = method_arg.name
+            if name in abi_args:
+                argument = abi_args.pop(name)
+                if isinstance(argument, dict):
+                    if hints.structs is None or name not in hints.structs:
+                        raise Exception(f"Argument missing struct hint: {name}. Check argument name and type")
+
+                    elements = hints.structs[name]["elements"]
 
-            args: list = []
-            # copy args so we don't mutate original
-            abi_args = dict(abi_args or {})
-            for method_arg in method.args:
-                name = method_arg.name
-                if name in abi_args:
-                    argument = abi_args.pop(name)
-                    if isinstance(argument, dict):
-                        if hints.structs is None or name not in hints.structs:
-                            raise Exception(f"Argument missing struct hint: {name}. Check argument name and type")
-
-                        elements = hints.structs[name]["elements"]
-
-                        argument_tuple = tuple(argument[field_name] for field_name, field_type in elements)
-                        args.append(argument_tuple)
-                    else:
-                        args.append(argument)
-
-                elif hints.default_arguments is not None and name in hints.default_arguments:
-                    default_arg = hints.default_arguments[name]
-                    if default_arg is not None:
-                        args.append(self.resolve(default_arg))
+                    argument_tuple = tuple(argument[field_name] for field_name, field_type in elements)
+                    args.append(argument_tuple)
                 else:
-                    raise Exception(f"Unspecified argument: {name}")
-            if abi_args:
-                raise Exception(f"Unused arguments specified: {', '.join(abi_args)}")
-            atc.add_method_call(
-                app_id,
-                method,
-                sender,
-                sp,
-                signer,
-                method_args=args,
-                on_complete=on_complete,
-                local_schema=local_schema,
-                global_schema=global_schema,
-                approval_program=approval_program,
-                clear_program=clear_program,
-                extra_pages=extra_pages or 0,
-                accounts=parameters.accounts,
-                foreign_apps=parameters.foreign_apps,
-                foreign_assets=parameters.foreign_assets,
-                boxes=encoded_boxes,
-                note=parameters.note.encode("utf-8") if isinstance(parameters.note, str) else parameters.note,
-                lease=encoded_lease,
-                rekey_to=parameters.rekey_to,
-            )
+                    args.append(argument)
+
+            elif hints.default_arguments is not None and name in hints.default_arguments:
+                default_arg = hints.default_arguments[name]
+                if default_arg is not None:
+                    args.append(self.resolve(default_arg))
+            else:
+                raise Exception(f"Unspecified argument: {name}")
+        if abi_args:
+            raise Exception(f"Unused arguments specified: {', '.join(abi_args)}")
+        return args
 
     def _method_matches(
         self,
         method: Method,
         args: ABIArgsDict | None,
         on_complete: transaction.OnComplete,
         call_config: au_spec.CallConfig,
@@ -1307,27 +1089,24 @@
         sig = method.get_signature()
         if sig not in self.app_spec.hints:
             return au_spec.MethodHints()
         return self.app_spec.hints[sig]
 
     def _execute_atc_tr(self, atc: AtomicTransactionComposer) -> TransactionResponse:
         result = self.execute_atc(atc)
-        return _tr_from_atr(atc, result)
+        return TransactionResponse.from_atr(result)
 
     def execute_atc(self, atc: AtomicTransactionComposer) -> AtomicTransactionResponse:
         return execute_atc_with_logic_error(
             atc,
             self.algod_client,
             approval_program=self.approval.teal if self.approval else self.app_spec.approval_program,
             approval_source_map=self._get_approval_source_map(),
         )
 
-    def _set_app_id_from_tx_id(self, tx_id: str) -> None:
-        self.app_id = get_app_id_from_tx_id(self.algod_client, tx_id)
-
     def get_signer_sender(
         self, signer: TransactionSigner | None = None, sender: str | None = None
     ) -> tuple[TransactionSigner | None, str | None]:
         """Return signer and sender, using default values on client if not specified
 
         Will use provided values if given, otherwise will fall back to values defined on client.
         If no sender is specified then will attempt to obtain sender from signer"""
@@ -1353,37 +1132,28 @@
         return resolved_signer, resolved_sender
 
     # TODO: remove private implementation, kept in the 1.0.2 release to not impact existing beaker 1.0 installs
     _resolve_signer_sender = resolve_signer_sender
 
 
 def substitute_template_and_compile(
-    algod_client: AlgodClient,
+    algod_client: "AlgodClient",
     app_spec: au_spec.ApplicationSpecification,
     template_values: au_deploy.TemplateValueMapping,
 ) -> tuple[Program, Program]:
     """Substitutes the provided template_values into app_spec and compiles"""
     template_values = dict(template_values or {})
     clear = au_deploy.replace_template_variables(app_spec.clear_program, template_values)
 
     au_deploy.check_template_variables(app_spec.approval_program, template_values)
     approval = au_deploy.replace_template_variables(app_spec.approval_program, template_values)
 
     return Program(approval, algod_client), Program(clear, algod_client)
 
 
-def get_app_id_from_tx_id(algod_client: AlgodClient, tx_id: str) -> int:
-    """Finds the app_id for provided transaction id"""
-    result = algod_client.pending_transaction_info(tx_id)
-    assert isinstance(result, dict)
-    app_id = result["application-index"]
-    assert isinstance(app_id, int)
-    return app_id
-
-
 def get_next_version(current_version: str) -> str:
     """Calculates the next version from `current_version`
 
     Next version is calculated by finding a semver like
     version string and incrementing the lower. This function is used by {py:meth}`ApplicationClient.deploy` when
     a version is not specified, and is intended mostly for convenience during local development.
 
@@ -1409,15 +1179,15 @@
     raise au_deploy.DeploymentFailedError(
         f"Could not auto increment {current_version}, please specify the next version using the version parameter"
     )
 
 
 def execute_atc_with_logic_error(
     atc: AtomicTransactionComposer,
-    algod_client: AlgodClient,
+    algod_client: "AlgodClient",
     wait_rounds: int = 4,
     approval_program: str | None = None,
     approval_source_map: SourceMap | None = None,
 ) -> AtomicTransactionResponse:
     """Calls {py:meth}`AtomicTransactionComposer.execute` on provided `atc`, but will parse any errors
     and raise a {py:class}`LogicError` if possible
 
@@ -1437,65 +1207,19 @@
                     program=approval_program,
                     source_map=approval_source_map,
                     **logic_error_data,
                 ) from ex
         raise ex
 
 
-def _create_metadata(
-    app_spec_note: au_deploy.AppDeployMetaData,
-    app_id: int,
-    created_round: int,
-    updated_round: int | None = None,
-    original_metadata: au_deploy.AppDeployMetaData | None = None,
-) -> au_deploy.AppMetaData:
-    app_metadata = au_deploy.AppMetaData(
-        app_id=app_id,
-        app_address=get_application_address(app_id),
-        created_metadata=original_metadata or app_spec_note,
-        created_round=created_round,
-        updated_round=updated_round or created_round,
-        **app_spec_note.__dict__,
-        deleted=False,
-    )
-    return app_metadata
-
-
 def _convert_call_parameters(args: CommonCallParameters | CommonCallParametersDict | None) -> CreateCallParameters:
     _args = args.__dict__ if isinstance(args, CommonCallParameters) else (args or {})
     return CreateCallParameters(**_args)
 
 
-def _convert_deploy_args(
-    _args: ABICallArgs | ABICallArgsDict | None,
-    note: au_deploy.AppDeployMetaData,
-    signer: TransactionSigner | None,
-    sender: str | None,
-) -> tuple[ABIMethod | bool | None, ABIArgsDict, CreateCallParameters]:
-    args = _args.__dict__ if isinstance(_args, ABICallArgs) else (_args or {})
-
-    # return most derived type, unused parameters are ignored
-    parameters = CreateCallParameters(
-        note=note.encode(),
-        signer=signer,
-        sender=sender,
-        suggested_params=args.get("suggested_params"),
-        lease=args.get("lease"),
-        accounts=args.get("accounts"),
-        foreign_assets=args.get("foreign_assets"),
-        foreign_apps=args.get("foreign_apps"),
-        boxes=args.get("boxes"),
-        rekey_to=args.get("rekey_to"),
-        extra_pages=args.get("extra_pages"),
-        on_complete=args.get("on_complete"),
-    )
-
-    return args.get("method"), args.get("args") or {}, parameters
-
-
 def get_sender_from_signer(signer: TransactionSigner | None) -> str | None:
     """Returns the associated address of a signer, return None if no address found"""
 
     if isinstance(signer, AccountTransactionSigner):
         sender = address_from_private_key(signer.private_key)  # type: ignore[no-untyped-call]
         assert isinstance(sender, str)
         return sender
@@ -1543,15 +1267,15 @@
             # Look for the last returned value in the log
             if not logs:
                 raise Exception("No logs")
 
             result = logs[-1]
             # Check that the first four bytes is the hash of "return"
             result_bytes = base64.b64decode(result)
-            if len(result_bytes) < 4 or result_bytes[:4] != ABI_RETURN_HASH:
+            if len(result_bytes) < len(ABI_RETURN_HASH) or result_bytes[: len(ABI_RETURN_HASH)] != ABI_RETURN_HASH:
                 raise Exception("no logs")
 
             raw_value = result_bytes[4:]
             abi_return_type = methods[i].returns.type
             if isinstance(abi_return_type, ABIType):
                 return_value = abi_return_type.decode(raw_value)
             else:
@@ -1610,27 +1334,7 @@
             case 3:
                 val = None
             case _:
                 raise NotImplementedError
 
         decoded_state[key] = val
     return decoded_state
-
-
-def _tr_from_atr(
-    atc: AtomicTransactionComposer, result: AtomicTransactionResponse, transaction_index: int = 0
-) -> TransactionResponse:
-    if result.abi_results and transaction_index in atc.method_dict:  # expecting an ABI result
-        abi_index = 0
-        # count how many of the earlier transactions were also ABI
-        for index in range(transaction_index):
-            if index in atc.method_dict:
-                abi_index += 1
-        return ABITransactionResponse(
-            **result.abi_results[abi_index].__dict__,
-            confirmed_round=result.confirmed_round,
-        )
-    else:
-        return TransactionResponse(
-            tx_id=result.tx_ids[transaction_index],
-            confirmed_round=result.confirmed_round,
-        )
```

## algokit_utils/application_specification.py

```diff
@@ -13,14 +13,15 @@
     "CallConfig",
     "DefaultArgumentDict",
     "DefaultArgumentType",
     "MethodConfigDict",
     "OnCompleteActionName",
     "MethodHints",
     "ApplicationSpecification",
+    "AppSpecStateDict",
 ]
 
 
 AppSpecStateDict: TypeAlias = dict[str, dict[str, dict]]
 """Type defining Application Specification state entries"""
 
 
@@ -58,15 +59,15 @@
     be resolved prior to calling some target method
     """
 
     source: DefaultArgumentType
     data: int | str | bytes | MethodDict
 
 
-StateDict = TypedDict(  # noqa: UP013  # can't convert as "global" is a reserved keyword
+StateDict = TypedDict(  # need to use function-form of TypedDict here since "global" is a reserved keyword
     "StateDict", {"global": AppSpecStateDict, "local": AppSpecStateDict}
 )
 
 
 @dataclasses.dataclass(kw_only=True)
 class MethodHints:
     """MethodHints provides hints to the caller about how to call the method"""
```

## algokit_utils/deploy.py

```diff
@@ -1,46 +1,63 @@
 import base64
 import dataclasses
 import json
 import logging
 import re
-from collections.abc import Callable, Iterable, Mapping
+from collections.abc import Iterable, Mapping, Sequence
 from enum import Enum
-from typing import TypeAlias
+from typing import TYPE_CHECKING, TypeAlias, TypedDict
 
 from algosdk import transaction
+from algosdk.atomic_transaction_composer import AtomicTransactionComposer, TransactionSigner
 from algosdk.logic import get_application_address
 from algosdk.transaction import StateSchema
-from algosdk.v2client.algod import AlgodClient
-from algosdk.v2client.indexer import IndexerClient
 
 from algokit_utils.application_specification import (
     ApplicationSpecification,
     CallConfig,
     MethodConfigDict,
     OnCompleteActionName,
 )
-from algokit_utils.models import Account, TransactionResponse
+from algokit_utils.models import (
+    ABIArgsDict,
+    ABIMethod,
+    Account,
+    CreateCallParameters,
+    TransactionResponse,
+)
+
+if TYPE_CHECKING:
+    from algosdk.v2client.algod import AlgodClient
+    from algosdk.v2client.indexer import IndexerClient
+
+    from algokit_utils.application_client import ApplicationClient
+
 
 __all__ = [
     "UPDATABLE_TEMPLATE_NAME",
     "DELETABLE_TEMPLATE_NAME",
     "NOTE_PREFIX",
+    "ABICallArgs",
+    "ABICreateCallArgs",
+    "ABICallArgsDict",
+    "ABICreateCallArgsDict",
     "DeploymentFailedError",
     "AppReference",
     "AppDeployMetaData",
     "AppMetaData",
     "AppLookup",
+    "Deployer",
     "DeployResponse",
     "OnUpdate",
     "OnSchemaBreak",
     "OperationPerformed",
     "TemplateValueDict",
     "TemplateValueMapping",
-    "check_app_and_deploy",
+    "get_app_id_from_tx_id",
     "get_creator_apps",
     "replace_template_variables",
 ]
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_INDEXER_MAX_API_RESOURCES_PER_ACCOUNT = 1000
@@ -131,15 +148,31 @@
     apps or discovering multiple app_ids
     """
 
     creator: str
     apps: dict[str, AppMetaData] = dataclasses.field(default_factory=dict)
 
 
-def get_creator_apps(indexer: IndexerClient, creator_account: Account | str) -> AppLookup:
+def _sort_by_round(txn: dict) -> tuple[int, int]:
+    confirmed = txn["confirmed-round"]
+    offset = txn["intra-round-offset"]
+    return confirmed, offset
+
+
+def _parse_note(metadata_b64: str | None) -> AppDeployMetaData | None:
+    if not metadata_b64:
+        return None
+    # noinspection PyBroadException
+    try:
+        return AppDeployMetaData.from_b64(metadata_b64)
+    except Exception:
+        return None
+
+
+def get_creator_apps(indexer: "IndexerClient", creator_account: Account | str) -> AppLookup:
     """Returns a mapping of Application names to {py:class}`AppMetaData` for all Applications created by specified
     creator that have a transaction note containing {py:class}`AppDeployMetaData`
     """
     apps: dict[str, AppMetaData] = {}
 
     creator_address = creator_account if isinstance(creator_account, str) else creator_account.address
     token = None
@@ -168,34 +201,20 @@
 
             created_transaction = next(
                 t
                 for t in transactions
                 if t["application-transaction"]["application-id"] == 0 and t["sender"] == creator_address
             )
 
-            def sort_by_round(txn: dict) -> tuple[int, int]:
-                confirmed = txn["confirmed-round"]
-                offset = txn["intra-round-offset"]
-                return confirmed, offset
-
-            transactions.sort(key=sort_by_round, reverse=True)
+            transactions.sort(key=_sort_by_round, reverse=True)
             latest_transaction = transactions[0]
             app_updated_at_round = latest_transaction["confirmed-round"]
 
-            def parse_note(metadata_b64: str | None) -> AppDeployMetaData | None:
-                if not metadata_b64:
-                    return None
-                # noinspection PyBroadException
-                try:
-                    return AppDeployMetaData.from_b64(metadata_b64)
-                except Exception:
-                    return None
-
-            create_metadata = parse_note(created_transaction.get("note"))
-            update_metadata = parse_note(latest_transaction.get("note"))
+            create_metadata = _parse_note(created_transaction.get("note"))
+            update_metadata = _parse_note(latest_transaction.get("note"))
 
             if create_metadata and create_metadata.name:
                 apps[create_metadata.name] = AppMetaData(
                     app_id=app_id,
                     app_address=get_application_address(app_id),
                     created_metadata=create_metadata,
                     created_round=app_created_at_round,
@@ -226,15 +245,16 @@
 class AppChanges:
     app_updated: bool
     schema_breaking_change: bool
     schema_change_description: str | None
 
 
 def check_for_app_changes(
-    algod_client: AlgodClient,
+    algod_client: "AlgodClient",
+    *,
     new_approval: bytes,
     new_clear: bytes,
     new_global_schema: StateSchema,
     new_local_schema: StateSchema,
     app_id: int,
 ) -> AppChanges:
     application_info = algod_client.application_info(app_id)
@@ -416,81 +436,321 @@
     app: AppMetaData
     create_response: TransactionResponse | None = None
     delete_response: TransactionResponse | None = None
     update_response: TransactionResponse | None = None
     action_taken: OperationPerformed = OperationPerformed.Nothing
 
 
-def check_app_and_deploy(
-    app: AppMetaData,
-    app_changes: AppChanges,
-    on_schema_break: OnSchemaBreak,
-    on_update: OnUpdate,
-    update_app: Callable[[], DeployResponse],
-    create_and_delete_app: Callable[[], DeployResponse],
-) -> DeployResponse:
-    if app_changes.schema_breaking_change:
-        logger.warning(f"Detected a breaking app schema change: {app_changes.schema_change_description}")
+@dataclasses.dataclass(kw_only=True)
+class ABICallArgs:
+    """Parameters used to update or delete an application when calling
+    {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
+
+    method: ABIMethod | bool | None = None
+    args: ABIArgsDict = dataclasses.field(default_factory=dict)
+    suggested_params: transaction.SuggestedParams | None = None
+    lease: bytes | str | None = None
+    accounts: list[str] | None = None
+    foreign_apps: list[int] | None = None
+    foreign_assets: list[int] | None = None
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
+    rekey_to: str | None = None
+
+
+@dataclasses.dataclass(kw_only=True)
+class ABICreateCallArgs(ABICallArgs):
+    """Parameters used to create an application when calling {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
+
+    extra_pages: int | None = None
+    on_complete: transaction.OnComplete | None = None
+
+
+class ABICallArgsDict(TypedDict, total=False):
+    """Parameters used to update or delete an application when calling
+    {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
+
+    method: ABIMethod | bool
+    args: ABIArgsDict
+    suggested_params: transaction.SuggestedParams
+    lease: bytes | str
+    accounts: list[str]
+    foreign_apps: list[int]
+    foreign_assets: list[int]
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]]
+    rekey_to: str
+
+
+class ABICreateCallArgsDict(TypedDict, ABICallArgsDict, total=False):
+    """Parameters used to create an application when calling {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
+
+    extra_pages: int | None
+    on_complete: transaction.OnComplete
+
+
+@dataclasses.dataclass(kw_only=True)
+class Deployer:
+    app_client: "ApplicationClient"
+    creator: str
+    signer: TransactionSigner
+    sender: str
+    existing_app_metadata_or_reference: AppReference | AppMetaData
+    new_app_metadata: AppDeployMetaData
+    on_update: OnUpdate
+    on_schema_break: OnSchemaBreak
+    create_args: ABICreateCallArgs | ABICreateCallArgsDict | None
+    update_args: ABICallArgs | ABICallArgsDict | None
+    delete_args: ABICallArgs | ABICallArgsDict | None
+
+    def deploy(self) -> DeployResponse:
+        """Ensures app associated with app client's creator is present and up to date"""
+        assert self.app_client.approval
+        assert self.app_client.clear
+
+        if self.existing_app_metadata_or_reference.app_id == 0:
+            logger.info(f"{self.new_app_metadata.name} not found in {self.creator} account, deploying app.")
+            return self._create_app()
+
+        assert isinstance(self.existing_app_metadata_or_reference, AppMetaData)
+        logger.debug(
+            f"{self.existing_app_metadata_or_reference.name} found in {self.creator} account, "
+            f"with app id {self.existing_app_metadata_or_reference.app_id}, "
+            f"version={self.existing_app_metadata_or_reference.version}."
+        )
+
+        app_changes = check_for_app_changes(
+            self.app_client.algod_client,
+            new_approval=self.app_client.approval.raw_binary,
+            new_clear=self.app_client.clear.raw_binary,
+            new_global_schema=self.app_client.app_spec.global_state_schema,
+            new_local_schema=self.app_client.app_spec.local_state_schema,
+            app_id=self.existing_app_metadata_or_reference.app_id,
+        )
 
-        if on_schema_break == OnSchemaBreak.Fail:
+        if app_changes.schema_breaking_change:
+            logger.warning(f"Detected a breaking app schema change: {app_changes.schema_change_description}")
+            return self._deploy_breaking_change()
+
+        if app_changes.app_updated:
+            logger.info(f"Detected a TEAL update in app id {self.existing_app_metadata_or_reference.app_id}")
+            return self._deploy_update()
+
+        logger.info("No detected changes in app, nothing to do.")
+        return DeployResponse(app=self.existing_app_metadata_or_reference)
+
+    def _deploy_breaking_change(self) -> DeployResponse:
+        assert isinstance(self.existing_app_metadata_or_reference, AppMetaData)
+        if self.on_schema_break == OnSchemaBreak.Fail:
             raise DeploymentFailedError(
                 "Schema break detected and on_schema_break=OnSchemaBreak.Fail, stopping deployment. "
                 "If you want to try deleting and recreating the app then "
                 "re-run with on_schema_break=OnSchemaBreak.ReplaceApp"
             )
-        if app.deletable:
+        if self.existing_app_metadata_or_reference.deletable:
             logger.info(
                 "App is deletable and on_schema_break=ReplaceApp, will attempt to create new app and delete old app"
             )
-        elif app.deletable is False:
+        elif self.existing_app_metadata_or_reference.deletable is False:
             logger.warning(
                 "App is not deletable but on_schema_break=ReplaceApp, "
                 "will attempt to delete app, delete will most likely fail"
             )
         else:
             logger.warning(
-                "Cannot determine if App is deletable but on_schema_break=ReplaceApp, " "will attempt to delete app"
+                "Cannot determine if App is deletable but on_schema_break=ReplaceApp, will attempt to delete app"
             )
-        return create_and_delete_app()
-    elif app_changes.app_updated:
-        logger.info(f"Detected a TEAL update in app id {app.app_id}")
+        return self._create_and_delete_app()
 
-        if on_update == OnUpdate.Fail:
+    def _deploy_update(self) -> DeployResponse:
+        assert isinstance(self.existing_app_metadata_or_reference, AppMetaData)
+        if self.on_update == OnUpdate.Fail:
             raise DeploymentFailedError(
                 "Update detected and on_update=Fail, stopping deployment. "
                 "If you want to try updating the app then re-run with on_update=UpdateApp"
             )
-        if app.updatable and on_update == OnUpdate.UpdateApp:
+        if self.existing_app_metadata_or_reference.updatable and self.on_update == OnUpdate.UpdateApp:
             logger.info("App is updatable and on_update=UpdateApp, will update app")
-            return update_app()
-        elif app.updatable and on_update == OnUpdate.ReplaceApp:
+            return self._update_app()
+        elif self.existing_app_metadata_or_reference.updatable and self.on_update == OnUpdate.ReplaceApp:
             logger.warning(
                 "App is updatable but on_update=ReplaceApp, will attempt to create new app and delete old app"
             )
-            return create_and_delete_app()
-        elif on_update == OnUpdate.ReplaceApp:
-            if app.updatable is False:
+            return self._create_and_delete_app()
+        elif self.on_update == OnUpdate.ReplaceApp:
+            if self.existing_app_metadata_or_reference.updatable is False:
                 logger.warning(
                     "App is not updatable and on_update=ReplaceApp, "
                     "will attempt to create new app and delete old app"
                 )
             else:
                 logger.warning(
                     "Cannot determine if App is updatable and on_update=ReplaceApp, "
                     "will attempt to create new app and delete old app"
                 )
-            return create_and_delete_app()
+            return self._create_and_delete_app()
         else:
-            if app.updatable is False:
+            if self.existing_app_metadata_or_reference.updatable is False:
                 logger.warning(
                     "App is not updatable but on_update=UpdateApp, "
                     "will attempt to update app, update will most likely fail"
                 )
             else:
                 logger.warning(
-                    "Cannot determine if App is updatable and on_update=UpdateApp, " "will attempt to update app"
+                    "Cannot determine if App is updatable and on_update=UpdateApp, will attempt to update app"
                 )
-            return update_app()
+            return self._update_app()
+
+    def _create_app(self) -> DeployResponse:
+        assert self.app_client.existing_deployments
+
+        method, abi_args, parameters = _convert_deploy_args(
+            self.create_args, self.new_app_metadata, self.signer, self.sender
+        )
+        create_response = self.app_client.create(
+            method,
+            parameters,
+            **abi_args,
+        )
+        logger.info(
+            f"{self.new_app_metadata.name} ({self.new_app_metadata.version}) deployed successfully, "
+            f"with app id {self.app_client.app_id}."
+        )
+        assert create_response.confirmed_round is not None
+        app_metadata = _create_metadata(self.new_app_metadata, self.app_client.app_id, create_response.confirmed_round)
+        self.app_client.existing_deployments.apps[self.new_app_metadata.name] = app_metadata
+        return DeployResponse(app=app_metadata, create_response=create_response, action_taken=OperationPerformed.Create)
+
+    def _create_and_delete_app(self) -> DeployResponse:
+        assert self.app_client.existing_deployments
+        assert isinstance(self.existing_app_metadata_or_reference, AppMetaData)
+
+        logger.info(
+            f"Replacing {self.existing_app_metadata_or_reference.name} "
+            f"({self.existing_app_metadata_or_reference.version}) with "
+            f"{self.new_app_metadata.name} ({self.new_app_metadata.version}) in {self.creator} account."
+        )
+        atc = AtomicTransactionComposer()
+        create_method, create_abi_args, create_parameters = _convert_deploy_args(
+            self.create_args, self.new_app_metadata, self.signer, self.sender
+        )
+        self.app_client.compose_create(
+            atc,
+            create_method,
+            create_parameters,
+            **create_abi_args,
+        )
+        delete_method, delete_abi_args, delete_parameters = _convert_deploy_args(
+            self.delete_args, self.new_app_metadata, self.signer, self.sender
+        )
+        self.app_client.compose_delete(
+            atc,
+            delete_method,
+            delete_parameters,
+            **delete_abi_args,
+        )
+        create_delete_response = self.app_client.execute_atc(atc)
+        create_response = TransactionResponse.from_atr(create_delete_response, 0)
+        delete_response = TransactionResponse.from_atr(create_delete_response, 1)
+        self.app_client.app_id = get_app_id_from_tx_id(self.app_client.algod_client, create_response.tx_id)
+        logger.info(
+            f"{self.new_app_metadata.name} ({self.new_app_metadata.version}) deployed successfully, "
+            f"with app id {self.app_client.app_id}."
+        )
+        logger.info(
+            f"{self.existing_app_metadata_or_reference.name} "
+            f"({self.existing_app_metadata_or_reference.version}) with app id "
+            f"{self.existing_app_metadata_or_reference.app_id}, deleted successfully."
+        )
+
+        app_metadata = _create_metadata(
+            self.new_app_metadata, self.app_client.app_id, create_delete_response.confirmed_round
+        )
+        self.app_client.existing_deployments.apps[self.new_app_metadata.name] = app_metadata
+
+        return DeployResponse(
+            app=app_metadata,
+            create_response=create_response,
+            delete_response=delete_response,
+            action_taken=OperationPerformed.Replace,
+        )
+
+    def _update_app(self) -> DeployResponse:
+        assert self.app_client.existing_deployments
+        assert isinstance(self.existing_app_metadata_or_reference, AppMetaData)
+
+        logger.info(
+            f"Updating {self.existing_app_metadata_or_reference.name} to {self.new_app_metadata.version} in "
+            f"{self.creator} account, with app id {self.existing_app_metadata_or_reference.app_id}"
+        )
+        method, abi_args, parameters = _convert_deploy_args(
+            self.update_args, self.new_app_metadata, self.signer, self.sender
+        )
+        update_response = self.app_client.update(
+            method,
+            parameters,
+            **abi_args,
+        )
+        app_metadata = _create_metadata(
+            self.new_app_metadata,
+            self.app_client.app_id,
+            self.existing_app_metadata_or_reference.created_round,
+            updated_round=update_response.confirmed_round,
+            original_metadata=self.existing_app_metadata_or_reference.created_metadata,
+        )
+        self.app_client.existing_deployments.apps[self.new_app_metadata.name] = app_metadata
+        return DeployResponse(app=app_metadata, update_response=update_response, action_taken=OperationPerformed.Update)
+
+
+def _create_metadata(
+    app_spec_note: AppDeployMetaData,
+    app_id: int,
+    created_round: int,
+    updated_round: int | None = None,
+    original_metadata: AppDeployMetaData | None = None,
+) -> AppMetaData:
+    return AppMetaData(
+        app_id=app_id,
+        app_address=get_application_address(app_id),
+        created_metadata=original_metadata or app_spec_note,
+        created_round=created_round,
+        updated_round=updated_round or created_round,
+        name=app_spec_note.name,
+        version=app_spec_note.version,
+        deletable=app_spec_note.deletable,
+        updatable=app_spec_note.updatable,
+        deleted=False,
+    )
+
+
+def _convert_deploy_args(
+    _args: ABICallArgs | ABICallArgsDict | None,
+    note: AppDeployMetaData,
+    signer: TransactionSigner | None,
+    sender: str | None,
+) -> tuple[ABIMethod | bool | None, ABIArgsDict, CreateCallParameters]:
+    args = _args.__dict__ if isinstance(_args, ABICallArgs) else (_args or {})
+
+    # return most derived type, unused parameters are ignored
+    parameters = CreateCallParameters(
+        note=note.encode(),
+        signer=signer,
+        sender=sender,
+        suggested_params=args.get("suggested_params"),
+        lease=args.get("lease"),
+        accounts=args.get("accounts"),
+        foreign_assets=args.get("foreign_assets"),
+        foreign_apps=args.get("foreign_apps"),
+        boxes=args.get("boxes"),
+        rekey_to=args.get("rekey_to"),
+        extra_pages=args.get("extra_pages"),
+        on_complete=args.get("on_complete"),
+    )
+
+    return args.get("method"), args.get("args") or {}, parameters
 
-    logger.info("No detected changes in app, nothing to do.")
 
-    return DeployResponse(app=app)
+def get_app_id_from_tx_id(algod_client: "AlgodClient", tx_id: str) -> int:
+    """Finds the app_id for provided transaction id"""
+    result = algod_client.pending_transaction_info(tx_id)
+    assert isinstance(result, dict)
+    app_id = result["application-index"]
+    assert isinstance(app_id, int)
+    return app_id
```

## algokit_utils/logic_error.py

```diff
@@ -1,12 +1,13 @@
 import re
 from copy import copy
-from typing import TypedDict
+from typing import TYPE_CHECKING, TypedDict
 
-from algosdk.source_map import SourceMap as AlgoSourceMap
+if TYPE_CHECKING:
+    from algosdk.source_map import SourceMap as AlgoSourceMap
 
 __all__ = [
     "LogicError",
     "parse_logic_error",
 ]
 
 LOGIC_ERROR = (
@@ -34,17 +35,18 @@
         "pc": int(match.group("pc")),
     }
 
 
 class LogicError(Exception):
     def __init__(
         self,
+        *,
         logic_error: Exception,
         program: str,
-        source_map: AlgoSourceMap,
+        source_map: "AlgoSourceMap",
         transaction_id: str,
         message: str,
         pc: int,
     ):
         self.logic_error = logic_error
         self.logic_error_str = str(logic_error)
         self.program = program
```

## algokit_utils/models.py

```diff
@@ -1,14 +1,17 @@
 import dataclasses
-from typing import Any
+from collections.abc import Sequence
+from typing import Any, Protocol, TypeAlias, TypedDict
 
+from algosdk import transaction
 from algosdk.abi import Method
+from algosdk.atomic_transaction_composer import AtomicTransactionResponse, TransactionSigner
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(kw_only=True)
 class Account:
     """Holds the private_key and address for an account"""
 
     private_key: str
     address: str
 
 
@@ -17,14 +20,34 @@
     """Response for a non ABI call"""
 
     tx_id: str
     """Transaction Id"""
     confirmed_round: int | None
     """Round transaction was confirmed, `None` if call was a from a dry-run"""
 
+    @staticmethod
+    def from_atr(result: AtomicTransactionResponse, transaction_index: int = 0) -> "TransactionResponse":
+        tx_id = result.tx_ids[transaction_index]
+        abi_result = next((r for r in result.abi_results if r.tx_id == tx_id), None)
+        if abi_result:
+            return ABITransactionResponse(
+                tx_id=tx_id,
+                raw_value=abi_result.raw_value,
+                return_value=abi_result.return_value,
+                decode_error=abi_result.decode_error,
+                tx_info=abi_result.tx_info,
+                method=abi_result.method,
+                confirmed_round=result.confirmed_round,
+            )
+        else:
+            return TransactionResponse(
+                tx_id=tx_id,
+                confirmed_round=result.confirmed_round,
+            )
+
 
 @dataclasses.dataclass(kw_only=True)
 class ABITransactionResponse(TransactionResponse):
     """Response for an ABI call"""
 
     raw_value: bytes
     """The raw response before ABI decoding"""
@@ -32,7 +55,71 @@
     """Decoded ABI result"""
     decode_error: Exception | None
     """Details of error that occurred when attempting to decode raw_value"""
     tx_info: dict
     """Details of transaction"""
     method: Method
     """ABI method used to make call"""
+
+
+ABIArgType = Any
+ABIArgsDict = dict[str, ABIArgType]
+
+
+class ABIReturnSubroutine(Protocol):
+    def method_spec(self) -> Method:
+        ...
+
+
+ABIMethod: TypeAlias = ABIReturnSubroutine | Method | str
+
+
+@dataclasses.dataclass(kw_only=True)
+class CommonCallParameters:
+    """Common transaction parameters used when making update, delete, opt_in, close_out or clear_state calls"""
+
+    signer: TransactionSigner | None = None
+    sender: str | None = None
+    suggested_params: transaction.SuggestedParams | None = None
+    note: bytes | str | None = None
+    lease: bytes | str | None = None
+    accounts: list[str] | None = None
+    foreign_apps: list[int] | None = None
+    foreign_assets: list[int] | None = None
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
+    rekey_to: str | None = None
+
+
+@dataclasses.dataclass(kw_only=True)
+class OnCompleteCallParameters(CommonCallParameters):
+    """Transaction parameters used when making any call to an Application"""
+
+    on_complete: transaction.OnComplete | None = None
+
+
+@dataclasses.dataclass(kw_only=True)
+class CreateCallParameters(OnCompleteCallParameters):
+    """Transaction parameters used when making a create call for Application"""
+
+    extra_pages: int | None = None
+
+
+class CommonCallParametersDict(TypedDict, total=False):
+    """Common transaction parameters used when making update, delete, opt_in, close_out or clear_state calls"""
+
+    signer: TransactionSigner
+    sender: str
+    suggested_params: transaction.SuggestedParams
+    note: bytes | str
+    lease: bytes | str
+
+
+class OnCompleteCallParametersDict(TypedDict, CommonCallParametersDict, total=False):
+    """Transaction parameters used when making any call to an Application"""
+
+    on_complete: transaction.OnComplete
+
+
+class CreateCallParametersDict(TypedDict, OnCompleteCallParametersDict, total=False):
+    """Transaction parameters used when making a create call for Application"""
+
+    extra_pages: int
```

## algokit_utils/network_clients.py

```diff
@@ -51,15 +51,15 @@
 def is_localnet(client: AlgodClient) -> bool:
     """Returns True if client genesis is `devnet-v1` or `sandnet-v1`"""
     params = client.suggested_params()
     return params.gen in ["devnet-v1", "sandnet-v1"]
 
 
 def is_sandbox(client: AlgodClient) -> bool:
-    warnings.warn("is_sandbox is deprecated, please use is_localnet instead", DeprecationWarning)
+    warnings.warn("is_sandbox is deprecated, please use is_localnet instead", DeprecationWarning, stacklevel=2)
     return is_localnet(client)
 
 
 def get_kmd_client_from_algod_client(client: AlgodClient) -> KMDClient:
     """Returns an {py:class}`algosdk.kmd.KMDClient` from supplied `client`
 
     Will use the same address as provided `client` but on port specified by `KMD_PORT` environment variable,
```

## Comparing `algokit_utils-1.0.3b2.dist-info/LICENSE` & `algokit_utils-1.0.4b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.0.3b2.dist-info/METADATA` & `algokit_utils-1.0.4b1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.0.3b2
+Version: 1.0.4b1
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

